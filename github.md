[Dmitrii Evdokimov's](/)

GitHub public projects 
======================

Мои открытые проекты на GitHub:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
[{{ repository.name }}](/{{ repository.name }}/ "Page")  
{{ repository.description }}
  {% endunless %}
{% endfor %}
