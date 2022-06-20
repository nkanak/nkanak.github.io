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

**Note for the 'first' authorship of a paper**: My laboratory used to follow the alphabetical order for the names of the authors, for the vast majority of our papers. Yes, I know, it does not make sense (and might I add silly), but, unfortunately, we cannot change the past (yet). For this reason, I added a <abbr class="badge" style="background-color:rgba(202, 60, 35, 0.925)">First Author</abbr> badge wherever I am the first author of a paper.


<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
