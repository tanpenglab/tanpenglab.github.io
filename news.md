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

  <!-- 帖子列表 + 卡片框 + 下划线链接 -->
  <div class="post-list" style="gap: 28px; display: flex; flex-direction: column;">
    {% for post in site.posts %}
      <!-- 每个帖子一个卡片框 -->
      <div style="border: 1px solid #e5e7eb; border-radius: 12px; padding: 20px 24px; background: #fff;">
        <p class="muted" style="margin: 0 0 6px; font-size: 0.86rem;">{{ post.date | date: "%b %-d, %Y" }}</p>
        <h3 style="margin: 0 0 8px; font-size: 1rem; font-weight: 600;">
          <!-- 正常无下划线，鼠标悬浮出现下划线 -->
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
