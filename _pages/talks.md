---
layout: page
permalink: /talks/
title: Talks
description: Selected recent talks.
nav: true
nav_order: 3
---

### Conferences

<div class="talks-list">
{% for talk in site.data.talks.conferences %}
<div class="talk-entry mb-3">
  <span class="text-muted">{{ talk.date }}</span>&ensp;
  <strong>{{ talk.type }}</strong>:
  <a href="{{ talk.url }}" target="_blank">{{ talk.title }}</a><br>
  <span class="text-muted">
    <a href="{{ talk.event_url }}" target="_blank">{{ talk.event }}</a>
    &mdash; {{ talk.location }}
  </span>
</div>
{% endfor %}
</div>

---

### Seminars

<div class="talks-list">
{% for talk in site.data.talks.seminars %}
<div class="talk-entry mb-3">
  <span class="text-muted">{{ talk.date }}</span>&ensp;
  <a href="{{ talk.url }}" target="_blank">{{ talk.title }}</a><br>
  <span class="text-muted">{{ talk.location }}</span>
</div>
{% endfor %}
</div>
