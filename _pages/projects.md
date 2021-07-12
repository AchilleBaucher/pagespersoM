---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

List of school, personal or internship projects.

{% include base_path %}

{% for proj in site.projects reversed %}
## [{{ proj.title }}]({{ base_path }}{{ proj.url }})
*{{ proj.what }}, {{ proj.date | date_to_string}}*

{{ proj.summary }}

[report]({{ base_path }}/files/{{ proj.report }})
- ---------------------------------------------
{% endfor %}
