---
title: Вырезки
---
Вырезки из старых газет и журналов
==================================

{% for paper in site.papers %}
<a name="#{{ paper.title | slugify }}"></a>
## [{{ paper.title }}]({{ paper.url }} "{{ paper.origin }}")

{{ paper.origin }}  
{{ paper.issued }}
{% endfor %}
