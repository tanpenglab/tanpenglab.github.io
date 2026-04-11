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

  <!-- 图片 + 下方小字 -->
  <div style="margin-bottom: 32px;">
    <img src="{{ '/assets/images/publication-flowchart.jpg' | relative_url }}"
         alt="Research overview flowchart"
         style="width: 100%; border-radius: 16px; object-fit: cover; display: block;">
    <div style="text-align: right; font-size: 0.65rem; color: #666; margin-top: 4px;">
      Cartoon adapted from Clark I. 2021 and Muus C. 2021, created using BioRender.
    </div>
  </div>

  <!-- 纯文本研究内容 -->
  <div style="display: flex; flex-direction: column; gap: 24px;">
    {% for item in site.data.research %}
    <div>
      <h3 style="font-size: 1rem; font-weight: 600; margin: 0 0 8px;">{{ item.title | upcase }}</h3>
      <p style="margin: 0; line-height: 1.6;">{{ item.summary }}</p>
    </div>
    {% endfor %}
  </div>
</section>
