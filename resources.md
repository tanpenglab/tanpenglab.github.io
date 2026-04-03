---
layout: default
title: Resources
permalink: /resources/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB PROTOCOLS</p>
    </div>
  </div>

  <!-- 去掉卡片框，纯文本展示，位置布局不变 -->
  <div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 32px;">
    {% for block in site.data.resources %}
      <div>
        <h3 style="font-size: 1rem; font-weight: 600; margin: 0 0 12px 0;">{{ block.category }}</h3>
        {% if block.items.size > 0 %}
        <ul style="list-style: none; padding: 0; margin: 0;">
          {% for item in block.items %}
            <li style="margin-bottom: 6px; font-size: 0.94rem; line-height: 1.5;">{{ item }}</li>
          {% endfor %}
        </ul>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</section>
