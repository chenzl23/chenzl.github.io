---
layout: page
permalink: /publications/
title: Publications
description: My published papers and preprints.
years: [2025, 2024, 2023, 2022, 2021]
nav: false
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

<div class="publications">
  <h2>Preprints</h2>
  {% bibliography -f preprint %}
</div>
