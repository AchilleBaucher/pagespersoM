---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Mes projets. Modifier et ajouter dans _projects. S'insiprer de publications et de portfolio.

{% include base_path %}

{% for proj in site.projects reversed %}
## [{{ proj.title }}]({{ base_path }}{{ proj.url }})
*{{ proj.date }}*

{{ proj.summary }}
* bp: {{ base_path }}

* bu: {{ site.base_url }}

* u: {{ site.url }}
* g: {{ site.github.url }}

[report]({{ base_path }}/files/{{ proj.report }})
{% endfor %}
