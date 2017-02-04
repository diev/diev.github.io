---
---
My public opensource projects on GitHub
=======================================

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
<a name="#{{ repository.name | slugify }}"></a>
[{{ repository.name }}](/{{ repository.name }}/ "Page")  
{{ repository.description }}
  {% endunless %}
{% endfor %}
