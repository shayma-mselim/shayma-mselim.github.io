---
layout: page
permalink: /publications/
title: publications
description: I'm currently still working on getting my first publication out into the world. Will update once it's out. :)
years: [2022]
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
