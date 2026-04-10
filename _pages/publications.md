---
layout: page
permalink: /publications/
title: publications
kicker: Research Output
description: Selected publications in cosmology and astrophysics.
years: [2025, 2023]
nav: true
nav_order: 2
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
