---
layout: page
permalink: /publications/
title: publications
description: Research publications in reverse chronological order. For the latest additions, see my <a href="https://scholar.google.com/citations?user=ZOyXeykAAAAJ&amp;hl=en">Google Scholar profile</a>.
years: [2026, 2024, 2023, 2022, 2020]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>
