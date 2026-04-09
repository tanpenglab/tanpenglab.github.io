---
layout: default
title: Home
---

<!-- 整个首页内容包在同一个 section 里，完全一体化 -->
<section class="section" style="max-width: 1200px; margin: 0 auto; padding: 20px 20px 0; box-sizing: border-box;">

  <!-- 顶部介绍文字 + 图片 -->
  <div class="hero-visual image-panel">
    <img src="{{ site.data.site.home_hero_image }}" alt="Tan Lab home image">
  </div>

  <!-- 居中副标题：和 Research Area 完全同样式，强制居中 -->
  <div style="width: 100%; text-align: center; margin: 24px 0;">
    <p class="eyebrow" style="margin: 0; display: inline-block;">
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

<style>
/* 全站导航统一：一行显示、不换行、不超出、间距拉开 */
.site-nav {
  display: flex !important;
  gap: 17px !important;
  justify-content: flex-end !important;
  flex-wrap: nowrap !important;
  white-space: nowrap !important;
  max-width: 100% !important;
  width: auto !important;
}

.site-nav a {
  font-size: 14.5px !important;
  white-space: nowrap !important;
}

/* 头部高度 */
.site-header {
  padding: 20px 0 !important;
}

/* 导航和 Research Area 完全对齐 */
.site-header .container {
  max-width: 1200px !important;
  margin: 0 auto !important;
  padding: 0 20px !important;
  width: 100% !important;
  box-sizing: border-box !important;
}

/* 手机端汉堡菜单修复 */
@media (max-width: 768px) {
  .site-nav {
    display: none !important;
  }
  .nav-open .site-nav {
    display: flex !important;
    flex-direction: column !important;
    position: absolute !important;
    top: 70px !important;
    left: 0 !important;
    right: 0 !important;
    background: #fff !important;
    padding: 20px !important;
    gap: 15px !important;
    z-index: 999 !important;
  }
}
</style>
