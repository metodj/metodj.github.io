---
layout: page
permalink: /research/
title: publications
description: 
years: [2021, 2020]
nav: true
nav_order: 1
---
<!-- _pages/research.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
