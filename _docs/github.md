---
---
Мои открытые проекты на GitHub
==============================

В алфавитном порядке:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
## [{{ repository.name }}](/{{ repository.name }}/ "Project page")

{{ repository.description }} - [GitHub]({{ repository.html_url }})

  {% endunless %}
{% endfor %}
