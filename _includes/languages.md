{% assign liste_languages = page.languages | split: ',' %}
<p>{% for l in liste_languages %}<code>{{ l }}</code> {% endfor %}</p>
