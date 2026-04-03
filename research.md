---
layout: default
title: Research
permalink: /research/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">RESEARCH OVERVIEW</p>
    </div>
  </div>

  <div class="stack-list">
    {% for item in site.data.research %}
      <article class="stack-card">
        <h3>{{ item.title | upcase }}</h3>
        <p>{{ item.summary }}</p>
      </article>
    {% endfor %}
  </div>

  <!-- 原来的 highlight 图片放在这里 -->
  <div style="margin-top: 32px;">
    <div class="image-panel publication-feature-figure">
      <img src="{{ '/assets/images/publication-flowchart.jpg' | relative_url }}" alt="Research overview flowchart" style="width: 100%; border-radius: 16px; object-fit: cover;">
    </div>
  </div>
</section>
