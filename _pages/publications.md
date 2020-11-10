---
layout: page
permalink: /publications/
title: publications
description: as  of Nov 2020
years: [2020, 2019, 2016, 2015, 2014, 2012, 1956, 1950, 1935, 1905]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
