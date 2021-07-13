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
*{{ proj.what }}, {{ proj.date | date: "%B %Y" }}*

{% if proj.logo %}<img align="left" height="160px" width="160px" style="margin-right:40px;" src="{{ base_path }}/images/{{ proj.logo }}" alt='logo' title={{ proj.logo_desc }}/>{% endif %}
{{ proj.summary }}{%if proj.report %} [Report]({{ base_path }}/files/{{ proj.report }}){% endif %}

{% if proj.languages %}
{% assign liste_languages = proj.languages | split: ',' %}
  {% for l in liste_languages %}`{{ l }}`{% endfor %}
{% endif %}

<br clear="left" />
- ---------------------------------------------
{% endfor %}
