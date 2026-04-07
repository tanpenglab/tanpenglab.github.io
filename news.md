---
layout: default
title: News
permalink: /news/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB NEWS</p>
    </div>
  </div>

  <!-- 纯文本新闻列表，无任何卡片框 -->
  <div class="post-list" style="gap: 28px; display: flex; flex-direction: column;">
    {% for post in site.posts %}
      <div>
        <p class="muted" style="margin: 0 0 6px; font-size: 0.86rem;">{{ post.date | date: "%b %-d, %Y" }}</p>
        <h3 style="margin: 0 0 8px; font-size: 1rem; font-weight: 600;">
          <!-- 鼠标悬浮显示下划线 -->
          <a href="{{ post.url | relative_url }}" style="color: var(--ink); text-decoration: none;"
            onmouseover="this.style.textDecoration='underline'"
            onmouseout="this.style.textDecoration='none'">
            {{ post.title }}
          </a>
        </h3>
        <p style="margin: 0; font-size: 0.94rem; line-height: 1.6; color: var(--muted);">
          {{ post.excerpt | strip_html | strip_newlines }}
        </p>
      </div>
    {% endfor %}
  </div>
</section>
