---
title: T0-Triatlon ervaringen
---

## Komende uitdagingen
{% assign wedstrijden = site.wedstrijden | sort: "date" %}
{% for wedstrijd in site.wedstrijden %}
* {{ wedstrijd.date }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endfor %}

## Uitslagen
