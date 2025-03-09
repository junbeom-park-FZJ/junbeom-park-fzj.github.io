---
layout: page
permalink: /presentation/
title: Presentations
description: 
nav: true
nav_order: 3
---


# Presentations
## A. Seminars and Lectures

<ol>
{% for paper in site._data.presentation_seminar %}
  <li>
    ({{paper.type}})  <b>{{ paper.title }}</b> <br>

    {% for author in paper.author %}
        {% if author.name == "Junbeom Park" %}
            <i> {{author.name}} </i>,
        {% else %}
            {{author.name}},
        {% endif %}
    {% endfor %}

    <br> {{ paper.location }} ({{ paper.year }}) {{ paper.city }} <br>
  </li>
{% endfor %}
</ol>

## B. Oral presentations at conferences
<ol>
{% for paper in site._data.presentation_oral %}
  <li>
    <b>{{ paper.title }}</b> <br>

    {% for author in paper.author %}
        {% if author.name == "Junbeom Park" %}
            <i> {{author.name}} </i>,
        {% else %}
            {{author.name}},
        {% endif %}
    {% endfor %}

    <br> {{ paper.location }} ({{ paper.year }}) {{ paper.city }} <br>
  </li>
{% endfor %}
</ol>

## C. Poster presentations at conferences

<ol>
{% for paper in site._data.presentation_poster %}
  <li>
    <b>{{ paper.title }}</b> <br>

    {% for author in paper.author %}
        {% if author.name == "Junbeom Park" %}
            <i> {{author.name}} </i>,
        {% else %}
            {{author.name}},
        {% endif %}
    {% endfor %}

    <br> {{ paper.location }} ({{ paper.year }}) {{ paper.city }} <br>
  </li>
{% endfor %}
</ol>