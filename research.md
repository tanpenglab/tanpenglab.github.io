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

  <!-- 直接展示纯文本，去掉 stack-card 四个框 -->
  <div style="margin-bottom: 32px;">
    {% for item in site.data.research %}
    <div style="margin-bottom: 24px;">
      <h3 style="font-size: 1rem; font-weight: 600; margin-bottom: 8px;">{{ item.title | upcase }}</h3>
      <p style="margin: 0; line-height: 1.6;">{{ item.summary }}</p>
    </div>
    {% endfor %}
  </div>

  <!-- 流程图放在纯文本下面 -->
  <div class="image-panel publication-feature-figure">
    <img src="{{ '/assets/images/publication-flowchart.jpg' | relative_url }}"
         alt="Research overview flowchart"
         style="width: 100%; border-radius: 16px; object-fit: cover;">
  </div>
</section>
