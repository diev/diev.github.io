---
---
Мои открытые проекты на GitHub
==============================

В алфавитном порядке:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
<section>
<a name="#{{ repository.name | slugify }}"></a>
## [{{ repository.name }}](/{{ repository.name }}/ "Страница проекта")

{{ repository.description }} - [GitHub]({{ repository.url }})
</section>
  {% endunless %}
{% endfor %}
