---
layout: page
permalink: /papers/
title: papers
order: 3
description: Publications by categories in reversed chronological order.
years: [2020, 2019, 2018, 2013, 2010, 2008, 2007, 2005]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
