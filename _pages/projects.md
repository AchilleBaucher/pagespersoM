---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Mes projets. Modifier et ajouter dans _projects. S'insiprer de publications et de portfolio.

{% for proj in site.projects reversed %}
## [{{ proj.title }}]({{ base_path }}{{ proj.url }})
*{{ proj.date }}*

{{ proj.summary }}
* bp: {{ base_path }}

* bu: {{ base_url }}

* u: {{ url }}

[report]({{ base_path }}/files/{{ proj.report }})
{% endfor %}
