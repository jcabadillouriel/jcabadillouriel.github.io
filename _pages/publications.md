---
layout: page
permalink: /publications/
title: Publications
description: Here go my publications and preprints in reversed chronological order.
years: [2022, 2021, 2020, 2019, 2018, 2017, 2015]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
