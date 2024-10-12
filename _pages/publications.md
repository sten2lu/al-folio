---
layout: page
permalink: /publications/
title: publications
description: A list of my selected publications.
years: [2024, 2023, 2022, 2019]
nav: true
---
<!-- _pages/publications.md -->
For a complete list of my publications I refer to my [GoogleScholar Profile](https://scholar.google.com/citations?user=3L6NkggAAAAJ&hl=de)
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
