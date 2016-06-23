---
title: T0-Triatlon ervaringen
---
## Komende uitdagingen
{% assign sortedwedstrijden = site.wedstrijden | sort: "date" %}
{% assign nu = site.time | date: '%s' %}
{% for wedstrijd in sortedwedstrijden %}
{% assign wedstrijddate = wedstrijd.date | date: '%s' %}
{% if wedstrijddate > nu %}
* {{ wedstrijd.date }} -- {{ wedstrijd.date | date: "%a, %b %d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

## Uitslagen
{% for wedstrijd in sortedwedstrijden %}
{% assign wedstrijddate = wedstrijd.date | date: '%s' %}
{% if wedstrijddate < nu %}
* {{ wedstrijd.date }} -- {{ wedstrijd.date | date: "%a, %b %d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

<img src="http://res.cloudinary.com/pdk/dpr_auto,w_auto,f_auto,q_auto/IMG_3854_rbwtfg">
