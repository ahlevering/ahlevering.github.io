---
layout: page
permalink: /publications/
title: Publications
description:
years_journal: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
# years_intconf: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015]
# years_natconf: [2023, 2022, 2021, 2017, 2016]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years_journal %}
  <!-- <h2 class="year">{{y}}</h2> -->
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

<!-- <br><br>
<div class="publications">
<h2>International Conferences</h2>
{%- for y in page.years_intconf %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f InternationalConf -q @*[year={{y}}]* %}
{% endfor %}

<br><br>
<div class="publications">
<h2>National Conferences</h2>
{%- for y in page.years_natconf %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f NationalConf -q @*[year={{y}}]* %}
{% endfor %}

</div> -->