---
title: T0-Triatlon ervaringen
---

## Komende uitdagingen
{% assign sortedwedstrijden = site.wedstrijden | sort: "title" %}
{% for wedstrijd in sortedwedstrijden %}
* {{ wedstrijd.date }} -- {{ wedstrijd.date | date: "%a, %b %d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endfor %}

## Uitslagen
{{site.time}}
