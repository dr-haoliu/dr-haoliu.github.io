---
layout: page
permalink: /publications/
title: Publications
description: publications by categories in reversed chronological order.
years: [2022, 2021, 2020, 2019, 2018, 2017, 2014]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

Note: JBI and JAMIA are leading health informatics journals with impact factors 8.000 and 7.942. <br>
AMIA (American Medical Informatics Association) is one of the top conferences in biomedical and health informatics.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
