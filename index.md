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

<img src="//res.cloudinary.com/pdk/dpr_auto,f_auto,q_auto,w_auto:150:900/IMG_3854_rbwtfg" sizes="100vw">

<img src="/images_api/dpr_auto,f_auto,q_auto,w_auto:150:900/IMG_3854_rbwtfg" sizes="100vw">
