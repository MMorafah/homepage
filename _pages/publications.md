---
layout: page
permalink: /publications/
title: Publications
description: Pre-prints, conference, journal, and workshop papers.
years: [2023, 2022, 2021]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">
<p> <strong>Disclaimer:</strong> This material is presented to ensure the timely dissemination of scholarly works. Copyright and all rights therein are retained by authors or by other copyright holders. All persons copying this information are expected to adhere to the terms invoked by each author's copyright. </p>
<p><mark>* denotes equal contribution and joint lead authorship</mark></p>

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
