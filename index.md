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

<img src="//res.cloudinary.com/pdk/dpr_auto,q_auto,w_auto:150:900/IMG_3854_rbwtfg" sizes="100vw">

<img src="data:image/jpeg;base64,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" sizes="100vw">
