---
title: T0-Triatlon ervaringen
---

## Komende uitdagingen
{% assign sortedwedstrijden = site.wedstrijden | sort: "date" %}
{% assign nu = site.time | date: '%s' %}
{% for wedstrijd in sortedwedstrijden %}
{% if wedstrijd.date > site.time %}
* {{ wedstrijd.date }} -- {{ wedstrijd.date | date: "%a, %b %d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

## Uitslagen
{{site.time  | date: '%s'}}
