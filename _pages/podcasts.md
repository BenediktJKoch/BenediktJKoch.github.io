---
layout: page
permalink: /podcasts/
title: podcasts
description: 
years: [History, Finance]
nav: false
heading: podcasts
---
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f podcasts -q @*[year={{y}}]* %}
{% endfor %}


</div>

