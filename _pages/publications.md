---
layout: page
permalink: /publications/
title: Publications
description: <h5>You may also checkout <a href="https://www.andrew.cmu.edu/user/kunz1/Publications.html"><u>publications before 2020</u></a>.</h5>
years: [2023,2022, 2021, 2020]
nav: true
nav_order: 2
---

<div class="publications">


{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}


</div>





