---
layout: default
title: Seminar
permalink: /seminar/
---

# Seminar & Talks

{% for item in site.data.seminars %}
<div style="margin-bottom: 2em;">
  <div style="font-weight: bold;">{{ item.date }} | {{ item.type }}</div>
  <div style="font-size: 1.1em; margin: 0.2em 0;">{{ item.title }}</div>
  <div>**Speaker:** {{ item.speaker }}</div>
  <div>{{ item.host }}</div>
  <div>{{ item.location }}</div>
</div>
{% endfor %}
