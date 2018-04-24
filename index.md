---
title: T0-Triatlon ervaringen
---
## Komende uitdagingen
{% assign sortedwedstrijden = site.wedstrijden | sort: "date" %}
{% assign nu = site.time | date: '%s' %}
{% for wedstrijd in sortedwedstrijden %}
{% assign wedstrijddate = wedstrijd.date | date: '%s' %}
{% if wedstrijddate > nu %}
* {{ wedstrijd.date | date: "%B %-d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

## Uitslagen
{% for wedstrijd in sortedwedstrijden %}
{% assign wedstrijddate = wedstrijd.date | date: '%s' %}
{% if wedstrijddate < nu %}
* {{ wedstrijd.date | date: "%B %-d, %Y" }} - <a href="{{ wedstrijd.url }}">{{ wedstrijd.title }}</a>
{% endif %}
{% endfor %}

<img data-src="https://res.cloudinary.com/pdk/dpr_auto,q_auto,w_auto:200:900/IMG_3854_rbwtfg" sizes="100vw" class="lazyload">
<img data-src="https://www.tixiv.be/img/w_200/IMG_3854_rbwtfg.jpg"  sizes="100vw" class="lazyload">
<img data-src="/IMG_3854_rbwtfg.jpg" sizes="100vw" class="lazyload">

Much better?


<img data-src="https://res.cloudinary.com/pdk/image/upload/c_fill,g_auto,ar_16:9/dpr_auto,q_auto/w_auto:breakpoints/IMG_3854_rbwtfg" sizes="100vw"  class="lazyload">
                                                                                                                                            <img data-src="https://www.tixiv.be/img/c_fill,g_auto,ar_16:9/dpr_auto,q_auto/w_auto:breakpoints/IMG_3854_rbwtfg" sizes="100vw"  class="lazyload">
