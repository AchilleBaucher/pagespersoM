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

<div><img align="left" width="150px" height="150px" style="margin-left 20px;" src="{{ base_url }}/images/{{ proj.logo }}" /> {{ proj.summary }}
</div>
<br><br>

{% if proj.languages %}
{% assign liste_languages = proj.languages | split: ',' %}
  {% for l in liste_languages %}`{{ l }}`{% endfor %}
{% endif %}


{%if proj.report %}[Report]({{ base_path }}/files/{{ proj.report }}){% endif %}
- ---------------------------------------------
{% endfor %}
