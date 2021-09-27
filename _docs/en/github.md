---
---
My public opensource projects on GitHub
=======================================

In alphabet order:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
<section>
<a name="#{{ repository.name | slugify }}"></a>
## [{{ repository.name }}](/{{ repository.name }}/ "Project page")

{{ repository.description }} - [GitHub]({{ repository.url }})
</section>
  {% endunless %}
{% endfor %}
