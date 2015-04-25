---
title: T0-Triatlon ervaringen
---
Juist gelijk alles da we doen is iedere start moeilijk.

De eerste looptraining, de eerste wedstijd, maar de eerste woorden op deze site.

Ik schat dat ik nu 1% klaar ben met de site, maar ik ben gestart!

Nu woord per woord dit hier verbeteren en we komen er wel.

* qsdfsdf
  * qsdsdf
  * qsdfdsf
* qdsfsdf
* sdqf

# Wedsttijden
{% if site.wedstrijden.size > 0  %}
{% for wedstrijd in site.wedstrijden %}
* <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endfor %}
{% endif %}
