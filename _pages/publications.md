---
layout: page
permalink: /publications/
title: publications
description: Publications in reversed chronological order. (* indicates equal contribution).
years: [2024, 2023, 2021]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
