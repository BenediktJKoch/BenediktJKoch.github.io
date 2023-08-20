---
layout: page
permalink: /publications/
title: publications
description: 
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<!-- <div class="publications">

{% bibliography -f {{ site.scholar.bibliography }} %}

</div> -->

<div class="publications">
    {% bibliography -f {{ site.scholar.bibliography }} %}
        {% for publication in site.bibliography %}
            <p>
                {% if publication.url %}
                    <a href="{{ publication.url }}" target="_blank">{{ publication.title }}</a>
                {% else %}
                    {{ publication.title }}
                {% endif %}
                - {{ publication.author }}, {{ publication.year }}
            </p>
        {% endfor %}
</div>


<!-- <div class="publications">
    {% bibliography -f {{ site.scholar.bibliography }} -q @*[key^={{ publications }}]* %}
        {% for publication in site.bibliography %}
            <p>
                {% if publication.url %}
                    <a href="{{ publication.url }}" target="_blank">{{ publication.title }}</a>
                {% else %}
                    {{ publication.title }}
                {% endif %}
                - {{ publication.author }}, {{ publication.year }}
            </p>
        {% endfor %}
</div> -->
