---
layout: page
permalink: /explorations/
title: Explorations
description: >
  A collection of exploratory projects beyond my primary research.
  These efforts reflect my curiosity about a wide range of physics, engineering, and computation.
nav: true
nav_order: 4
---

{% assign explorations = site.explorations | sort: 'date' | reverse %}
{% for item in explorations %}

<div class="d-flex align-items-start mb-4">
  {% if item.thumbnail %}
  <div style="flex: 0 0 200px; margin-right: 1.5rem; align-self: stretch; display: flex; align-items: center; background: transparent;">
    <img src="{% if item.thumbnail contains '://' %}{{ item.thumbnail }}{% else %}/{{ item.thumbnail }}{% endif %}" class="rounded z-depth-1" style="width: 200px; height: 100%; object-fit: contain; min-height: 80px;" alt="{{ item.title }}">
  </div>
  {% endif %}
  <div>
    <h5 class="mb-1"><a href="{{ item.url | relative_url }}">{{ item.title }}</a></h5>
    {% if item.date %}<small class="text-muted">{{ item.date | date: "%Y.%m" }}</small>{% endif %}
    <p class="mt-1 mb-1">{{ item.description }}</p>
  </div>
</div>
{% endfor %}
