[Dmitrii Evdokimov's](/)

GitHub public projects 
======================

Мои открытые проекты на GitHub:

{% for repository in site.github.public_repositories %}
  {% unless repository.fork %}
[{{ repository.name }}](/{{ repository.name }}/ "Page") - [View]({{ repository.html_url }} "GitHub") | [Downloads]({{ repository.releases_url }} "Releases")  
{{ repository.description }}
  {% endunless %}
{% endfor %}
