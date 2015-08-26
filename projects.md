---
layout: page
title: Projects
permalink: /projects/
---

Some of my projects are listed below.

<section class="grid-wrapper">
  <div class="left-column">
    <strong>Tools</strong><br />
    {% for page in site.pages %}
      {% if page.title %}
        {% if page.categories contains 'project' %}
          <a href="{{ page.url }}">{{ page.title }}</a><br />
        {% endif %}
      {% endif %}
    {% endfor %}
  </div>

  <div class="middle-column">
    <strong>Spaces & Events</strong><br />
    {% for page in site.pages %}
      {% if page.title %}
        {% if page.categories contains 'environment' %}
          <a href="{{ page.url }}">{{ page.title }}</a><br />
        {% endif %}
      {% endif %}
    {% endfor %}
  </div>

  <div class="right-column">
    <strong>Gadgets</strong><br />
    {% for page in site.pages %}
      {% if page.title %}
        {% if page.categories contains 'gadget' %}
          <a href="{{ page.url }}">{{ page.title }}</a><br />
        {% endif %}
      {% endif %}
    {% endfor %}
  </div>
</section>

<!--
<br />

<section class="grid-wrapper">
  <div class="left-column">
    <strong>Videos</strong><br />
    {% for page in site.pages %}
      {% if page.title %}
        {% if page.categories contains 'video' %}
          <a href="{{ page.url }}">{{ page.title }}</a><br />
        {% endif %}
      {% endif %}
    {% endfor %}
  </div>

  <div class="middle-column">

  </div>

  <div class="right-column">

  </div>
</section>
-->
