---
layout: page
permalink: /publications/
title: publications
description:
years: [2023, 2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>

<!-- code={ https://github.com/shmsw25/FActScore }, -->
<!-- code={ https://github.com/alrope123/z-icl }, -->
<!-- code={ https://github.com/Alrope123/rethinking-demonstrations }, -->