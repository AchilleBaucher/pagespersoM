---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Mes projets. Modifier et ajouter dans _projects. S'insiprer de publications et de portfolio.

{% for proj in site.projects reversed %}
## [{{ proj.title }}]({{ proj.url }})
*{{ proj.date }}*

{{ proj.summary }}

[report](/files/{{ proj.report }})
{% endfor %}
