---
layout: page
permalink: /publications/
title: publications
description: 
years: [2022, 2021, 2020, 2019, 2016]
nav: true
nav_order: 2
---
For my publications, you can also check my profile on <a href="https://scholar.google.com/citations?user=rX-SfF8AAAAJ">Google Scholar</a>.

<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
