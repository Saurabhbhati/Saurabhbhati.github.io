---
layout: page
permalink: /publications/
title: publications
#description: publications by categories in chronological order.
years: [2022,2021,2020,2019,2018,2017]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="Jounral publications">
years: [2022,2020]
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f journal_papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<div class="Conference proceedings">
years: [2021,2020,2019,2018,2017]
{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
