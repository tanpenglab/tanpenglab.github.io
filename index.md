---
layout: default
title: Home
---

<!-- 首页整体区域 -->
<section class="section">

  <!-- 顶部主图 -->
  <div class="hero-visual image-panel">
    <img src="{{ site.data.site.home_hero_image }}" alt="Tan Lab home image">
  </div>

  <!-- 副标题标语 -->
  <div class="hero-tagline" style="text-align: center; margin: 24px 0;">
    <p class="eyebrow">Systems Approaches to Gut Biology and Disease</p>
  </div>

  <!-- 实验室简介 -->
  <div class="hero-copy" style="margin: 24px 0 48px;">
    <h1 style="text-align: justify; font-size: 1.1rem; line-height: 1.6; font-weight: normal;">
      {{ site.data.site.intro }}
    </h1>
    <div class="cta-row" style="margin-top: 20px; display: flex; gap: 1rem; justify-content: center; flex-wrap: wrap;">
      <a class="button" href="{{ '/research/' | relative_url }}">Explore Research</a>
      <a class="button secondary" href="{{ '/publications/' | relative_url }}">View Publications</a>
    </div>
  </div>

  <!-- 研究方向标题栏 -->
  <div class="section-head">
    <p class="eyebrow">Research Area</p>
    <a class="text-link" href="{{ '/research/' | relative_url }}">Read More</a>
  </div>

  <!-- 研究方向卡片 -->
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

  <!-- 底部整幅图片 -->
  <div style="margin-top: 36px;">
    <img
      src="/assets/images/home-page-logo.png"
      alt="Lab logo banner"
      style="width: 100%; height: auto; border-radius: 16px; object-fit: cover; display: block;"
    >
  </div>

</section>
