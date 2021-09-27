---
title: Paper Cuts
---
A set of old paper cuts
=======================

Mostly in the Russian language.

{% for paper in site.papers %}
<a name="#{{ paper.title | slugify }}"></a>[{{ paper.title }}]({{ paper.url }} "{{ paper.origin }}")  
*{{ paper.origin }}*  
*{{ paper.issued }}*
{% endfor %}
