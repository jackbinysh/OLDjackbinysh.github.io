---
layout: page
permalink: /publications/
title: Publications
bannerimage: banner.png
years: [2020,2019,2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
