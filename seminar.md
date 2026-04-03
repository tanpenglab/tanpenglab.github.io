---
layout: default
title: Lab Seminar
permalink: /seminar/
---

<section class="page-hero page-hero--compact">
  <p class="eyebrow">LAB SEMINAR</p>
  <p>Invited speakers and lab presentations</p>
</section>

<section class="section">
  <div class="pub-list">
    {% for item in site.data.seminars %}
    <article class="pub-item">
      <div class="pub-meta">
        <!-- 只保留日期，删掉了类型 -->
        <span class="pub-date">{{ item.date }}</span>
      </div>
      <div class="pub-title">
        {{ item.title }}
      </div>
      <!-- Speaker 不加粗，带链接 -->
      <div>Speaker: <a href="{{ item.link }}" target="_blank">{{ item.speaker }}</a></div>
      <div>{{ item.host }}</div>
      <div>{{ item.location }}</div>
    </article>
    {% endfor %}
  </div>
</section>
