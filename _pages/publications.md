---
layout: page
permalink: /publications/
title: Publications
description: You can find all the publications here.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013, 2012, 2011, 2004]
nav: true
nav_order: 1
link: https://pubmed.ncbi.nlm.nih.gov/?term=Lo-Ciganic
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
