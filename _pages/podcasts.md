---
layout: page
permalink: /podcasts/
title: podcasts
description: 
years: [History, News, Finance, Economics]
nav: false
heading: podcasts
---
<div class="publications">


I am a huge podcast fan. Below you can find a list of some of my favorite podcasts. If you know any good ones, don't hesitate to contact me!


{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f podcasts -q @*[year={{y}}]* %}
{% endfor %}

</div>

