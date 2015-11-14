---
layout: default
title: Poetry
permalink: /writing/poetry/
categories: writing
order: 0
---

<div class="home">
  <strong>Poetry</strong><br />
  {% assign sorted_pages = (site.pages | sort: 'order') %}
  {% for page in sorted_pages reversed | sort: 'order' %}
    {% if page.title %}
      {% if page.categories contains 'poetry' %}
        <a href="{{ page.url }}">{{ page.title }}</a><br />
      {% endif %}
    {% endif %}
  {% endfor %}
</div>
