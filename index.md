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


<img sizes="100vw" srcset="http://res.cloudinary.com/demo/w_auto:100:320/bike.jpg	320w,
http://res.cloudinary.com/demo/w_auto:100:512/bike.jpg	512w,
http://res.cloudinary.com/demo/w_auto:100:640/bike.jpg	640w,
http://res.cloudinary.com/demo/w_auto:100:1024/bike.jpg	1024w,
http://res.cloudinary.com/demo/w_auto:100:1280/bike.jpg	1280w,
http://res.cloudinary.com/demo/w_auto:100:2048/bike.jpg	2048w" src="http://res.cloudinary.com/demo/w_auto:100:1024/bike.jpg" alt="To each according to his Smiling girl with a bike"/>
