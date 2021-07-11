---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Mes projets. Modifier et ajouter dans _projects. S'insiprer de publications et de portfolio.

{% for post in site.projects reversed %}
  * {{ post.title }}
{% endfor %}
