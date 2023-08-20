---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

<!-- {% bibliography -f {{ site.scholar.bibliography }} %} -->

{% for entry in site.data.bibliography %}
  {% include bibliography.html entry=entry %}
{% endfor %}

</div>
