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

<img sizes="80vw" src="https://lh3.googleusercontent.com/ZB1eSowcybNuoALeIRWiXMOpIpIYi4ZNbkeMSVN05-nNaNTCHqnqdspd3avVvs0y9ZUB2asWHDTBIt4OzDakUkbgO1AsU82n10_-lsbRfBd3P53U8StXavdLYO-36xIeGs6vjMI9xYM5GSlgNcz_NOwr2qZOWPxGTjz_ayms1OPW7J0JgqLW6Quv08TLo0KlWc9qG8o3kEmIjqxU7-wTkOAa8QqNWUeFx2X6yBx6GhSfaI-wo1j9pkyU9T9hxqLPugMwHNllf1eLC_LU7857QFJW1L_VkQIAo-wQ4j-0TCFE0jfuqDMMUIyBVnyjlQifRb3nqP9EkYFLWaH_5E-xafQLKOvaxLtadH8HAOwQlZZVkgFOGWB-8xp5nsM5LGOqRLKibPQzhZb5zFAHl_xqHA2ZBHoz3-TJcbYleiF13PYCF2wjYLRIe9adi0RkKeC3J1qeWOdkDokTRTo7MXS4YoIqcMs-rffWwQEEgoiQPLlumTgyHb6YQHIM6KeWIUHjgxujx_N5IGEqQZxHIjbo9OitRRXSIEHWiLzPgVwqM_vmixUaWoLk9pcSavkHQ5bU6hl8AeTRx42JDLuNCDh1mHvH986NEXbv=w1309-h979-no">
