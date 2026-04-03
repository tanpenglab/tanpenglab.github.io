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
        <!-- 这里去掉了加粗样式，普通文本显示 -->
        <span>{{ item.type }}</span>
        <span>•</span>
        <span class="pub-date">{{ item.date }}</span>
      </div>
      <div class="pub-title">
        {{ item.title }}
      </div>
      <!-- Speaker 带链接 -->
      <div><strong>Speaker:</strong> <a href="{{ item.link }}" target="_blank">{{ item.speaker }}</a></div>
      <div>{{ item.host }}</div>
      <div>{{ item.location }}</div>
    </article>
    {% endfor %}
  </div>
</section>
