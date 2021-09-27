---
title: Clippings
---
Clippings from old newspapers and magazines
===========================================

Mostly in the Russian language.

{% for paper in site.papers %}
<section>
<a name="#{{ paper.title | slugify }}"></a>
## [{{ paper.title }}]({{ paper.url }} "{{ paper.origin }}")

{{ paper.origin }}  
{{ paper.issued }}
</section>
{% endfor %}
