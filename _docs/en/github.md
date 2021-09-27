---
---
My public opensource projects on GitHub
=======================================

In alphabet order:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
<a name="#{{ repository.name | slugify }}"></a>
## [{{ repository.name }}](/{{ repository.name }}/ "Project page")

{{ repository.description }} - [GitHub]({{ repository.html_url }})
  {% endunless %}
{% endfor %}
