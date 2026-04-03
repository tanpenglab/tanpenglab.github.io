---
layout: default
title: Resources
permalink: /resources/
---

<!-- 顶部加 LAB PROTOCOLS，样式和 LAB SEMINAR 完全一致 -->
<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB PROTOCOLS</p>
    </div>
  </div>

  <div class="resource-grid">
    {% for block in site.data.resources %}
      <article class="resource-card">
        <h3>{{ block.category }}</h3>
        {% if block.items.size > 0 %}
        <ul>
          {% for item in block.items %}
            <li>{{ item }}</li>
          {% endfor %}
        </ul>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
