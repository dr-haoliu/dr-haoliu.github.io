---
layout: page
permalink: /publications/
title: Publications
description: publications by categories in reversed chronological order.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2014]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

Note: <b>JBI</b> and <b>JAMIA</b> are leading health informatics journals with impact factors <b>8.000</b> and <b>7.942</b> (2022). <br>
<b>AMIA</b> (American Medical Informatics Association) is one of the top conferences in biomedical and health informatics.

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
