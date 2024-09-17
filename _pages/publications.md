---
layout: page
permalink: /publications/
title: publications
description: ordered in reversed chronological order.
years: [2024, 2023, 2022]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->

<p>For a longer list, please refer to the PI's <a href="https://scholar.google.com/citations?user=uH74dcgAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar page</a>.</p>

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
