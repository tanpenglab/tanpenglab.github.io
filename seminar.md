---
layout: default
title: Lab Seminar
permalink: /seminar/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB SEMINAR</p>
      <p>Invited speakers and lab presentations</p>
    </div>
  </div>

  <div class="pub-list">
    {% for item in site.data.seminars %}
    <article class="pub-item">
      <div class="pub-meta">
        <span class="pub-date">{{ item.date }}</span>
      </div>
      <div class="pub-title">
        {{ item.title }}
      </div>
      <div>Speaker: <a href="{{ item.link }}" target="_blank">{{ item.speaker }}</a></div>
      <div>{{ item.host }}</div>
      <div>{{ item.location }}</div>
    </article>
    {% endfor %}
  </div>
</section>
