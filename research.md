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

  <!-- 图片 + 右下角小字 -->
  <div style="position: relative; margin-bottom: 32px;">
    <img src="{{ '/assets/images/publication-flowchart.jpg' | relative_url }}"
         alt="Research overview flowchart"
         style="width: 100%; border-radius: 16px; object-fit: cover; display: block;">
    <div style="position: absolute; right: 12px; bottom: 8px; font-size: 0.65rem; color: #666;">
      Cartoon adapted from I Clark et al. Science 2021 and C Muus et al. Nature Medicine 2021, created using BioRender.
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
