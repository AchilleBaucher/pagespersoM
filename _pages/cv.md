---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}
Pdf versions: [EN]({{ base_path }}/files/cv_en.pdf), [FR]({{ base_path }}/files/cv_fr.pdf)


Education
======
* Erasmus Exchange Semester, [University of Oslo](https://www.uio.no/), *Spring 2021*
  * *[Computational Statistics](https://www.uio.no/studier/emner/matnat/math/STK4051/index-eng.html#course_content), [Probabilistic Graphical Models](https://www.uio.no/studier/emner/matnat/math/STK4290/v21/final-curriculum.html), [Statistical Model Selection](https://www.uio.no/studier/emner/matnat/math/STK4160/index-eng.html#course_content)*
* Ingineering Cursus in Applied Mathematics and Computer Science, [Polytech Sorbonne](https://www.polytech.sorbonne-universite.fr/formations/mathematiques-appliques-et-informatique), *2016 - ongoing*
  * *Algorithmic, Numerical Analysis, Computing, Cryptography, Databases, Data Analysis, Modelling, High Performance Computing, Continous & Combinatorial Optimisation, Machine Learning, Signal Processing, Stochastic Processes*
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
  * *{{ proj.what }}, {{ proj.date | date:"%B %Y" }}*{%if proj.institution %}{%if proj.institution_url %}, [{{ proj.institution }}]({{ proj.institution_url }}){% else %}, {{ proj.institution }} {% endif %}{% endif %}
{% endif %}
{% endfor %}

Programming skills
======
* Python
* R
* C++
* Matlab
* LateX
* Linux

Languages
======
* French (native)
* English (B2)
* Chinese (HSK1)

Associative Experience
======
* Lupalytech, 2019-2020
  * Co-created an association to support various ecological projects.
  * Hired new students, helped to design and supervised projects, workshops, etc.
* Rafisto (Enactus project), 2018-2019
  * Co-created and led an associative project
  * Organized workshops to repair devices
  * Tried to sensibilise students about planned obsollescence
* Scout, 2010-2016
  * Organized diverse projects: buildings, camps
  * Led a team of 8 members during one year
