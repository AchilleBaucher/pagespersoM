---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Erasmus Exchange Semester, [University of Oslo](https://www.uio.no/), *Spring 2021*
  * *Probabilistic Graphical Models, Computational Statistics, Statistical Model Selection*
* Applied Mathematics and Computer Science, [Polytech Sorbonne](https://www.polytech.sorbonne-universite.fr/), *2017 - ongoing*
  * *Analysis, Modelling, Optimisation, Data Analysis, Algorithmic, Computing, Databases, Graph Theory, High Performance Computing, Machine Learning, Cryptography*
* Scientific Baccalaureate, Lycée Hoche de Versailles, *2016*

Work experience
======
{% for proj in site.projects reversed%}
{% if proj.type == 'internship' %}
* {{ proj.date | date: "%B %Y"}}: [{{ proj.title }}]({{ base_path }}{{ proj.url }})
  * *{{ proj.what }}* {%if proj.institution %}{%if proj.institution_url %}*, [{{ proj.institution }}]({{ proj.institution_url }})*{% else %} {{ proj.institution }} {% endif %}{% endif %}
  * {{proj.summary}}
{% endif %}
{% endfor %}

Other projects
======
{% for proj in site.projects reversed %}
{% if proj.type != 'internship' %}
* [{{ proj.title }}]({{ base_path }}{{ proj.url }})
  * *{{ proj.what }}*{%if proj.institution %}{%if proj.institution_url %}*, [{{ proj.institution }}]({{ proj.institution_url }})*{% else %} {{ proj.institution }} {% endif %}{% endif %}*, {{ proj.date | date_to_string}}*
{% endif %}
{% endfor %}

Programming skills
======
* Python
* R
* C++
* Matlab
* LateX

Languages
======
* French (native)
* English (B2)
* Chinese (HSK1)

Associative Experience
======
* Lupalytech, 2019-2020
  * Co-created an association to support and supervise various ecological projects
* Rafisto, 2018-2019
  * Organized workshops to repair electronic devices
* Scout, 2010-2016
  * ...
