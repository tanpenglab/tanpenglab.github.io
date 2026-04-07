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

  <!-- 帖子列表，每个帖子一个卡片框 -->
  <div class="post-list" style="gap: 28px; display: flex; flex-direction: column;">
    {% for post in site.posts %}
      <!-- 👇 这里给每个帖子加了卡片框 -->
      <div style="
        border: 1px solid #e5e7eb;
        border-radius: 12px;
        padding: 20px 24px;
        background: #ffffff;
        transition: all 0.2s ease;
      ">
        <p class="muted" style="margin: 0 0 6px; font-size: 0.86rem;">{{ post.date | date: "%b %-d, %Y" }}</p>
        <h3 style="margin: 0 0 8px; font-size: 1rem; font-weight: 600;">
          <a href="{{ post.url | relative_url }}" style="color: var(--ink); text-decoration: none;">
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
