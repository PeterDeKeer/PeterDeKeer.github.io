---
title: T0-Triatlon ervaringen
---

## Komende uitdagingen
{% assign sortedwedstrijden = site.wedstrijden | sort: "date" %}
{% for wedstrijd in sortedwedstrijden %}
{% if 10 > 9 %}
* {{ wedstrijd.date }} -- {{ wedstrijd.date | date: "%a, %b %d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

## Uitslagen
{{site.time}}
