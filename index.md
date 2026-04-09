---
layout: default
title: Home
---

<!-- 整个首页内容包在同一个 section 里，完全一体化 -->
<section class="section">

  <!-- 顶部介绍文字 + 图片 -->
  <div class="hero-visual image-panel">
    <img src="{{ site.data.site.home_hero_image }}" alt="Tan Lab home image">
  </div>

  <!-- 居中副标题：100% 强制居中，无任何偏移 -->
  <div style="width: 100%; text-align: center; margin: 24px 0;">
    <p class="eyebrow" style="margin: 0 auto; text-align: center; width: 100%;">
      Systems Approaches to Gut Biology and Disease
    </p>
  </div>

  <div class="hero-copy" style="margin: 24px 0 48px 0;">
    <h1 style="text-align: justify; font-size: 1.1rem; line-height: 1.6; font-weight: normal;">
      {{ site.data.site.intro }}
    </h1>
    <div class="cta-row" style="margin-top: 20px;">
      <a class="button" href="{{ '/research/' | relative_url }}">Explore Research</a>
      <a class="button secondary" href="{{ '/publications/' | relative_url }}">View Publications</a>
    </div>
  </div>

  <!-- Research Area 紧接在下面，无间隔分段 -->
  <div class="section-head">
    <div>
      <p class="eyebrow">Research Area</p>
    </div>
    <a class="text-link" href="{{ '/research/' | relative_url }}">Read More</a>
  </div>

  <div class="grid grid-2">
    {% for item in site.data.home_research %}
      <article class="card research-card">
        <img src="{{ item.image }}" alt="{{ item.title }}">
        <div class="card-body">
          <h3>{{ item.title }}</h3>
          <p>{{ item.description }}</p>
        </div>
      </article>
    {% endfor %}
  </div>

  <div style="margin-top: 36px; width: 100%;">
    <img src="/assets/images/home-page-logo.png"
         style="width: 100%; height: auto; border-radius: 16px; object-fit: cover; display: block;">
  </div>

</section>
