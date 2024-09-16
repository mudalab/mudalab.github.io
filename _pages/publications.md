---
layout: page
permalink: /publications/
title: publications
description: Ordered in reversed chronological order. For a longer list, please refer to <a href="https://scholar.google.com/citations?user=uH74dcgAAAAJ" target="_blank">here</a>.
years: [2024, 2023, 2022, 2021]
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
