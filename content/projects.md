---
layout: projects
title: Projects
permalink: '/projects/'
---

{% for item in site.projects %}
  <p><a href="{{ item.url }}">{{ item.title }}</a></p>
{% endfor %}
