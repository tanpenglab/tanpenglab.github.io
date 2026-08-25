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

  <!-- ========== 新增：Our lab is supported by 资助Logo区域 ========== -->
  <div style="margin-top: 64px; padding-top:32px; border-top:1px solid #e5e7eb;">
    <p class="eyebrow" style="margin-bottom:24px;">Our lab is supported by:</p>
    <div style="display:flex; flex-wrap:wrap; gap:2rem; align-items:center;">
      <!-- 替换为你的实际logo路径，可继续复制增加 -->
      <img src="/assets/funding/funder1.png" alt="Funder 1" style="height:56px; width:auto;">
      <img src="/assets/funding/funder2.png" alt="Funder 2" style="height:56px; width:auto;">
      <img src="/assets/funding/funder3.png" alt="Funder 3" style="height:56px; width:auto;">
    </div>
  </div>
  <!-- ========== 新增结束 ========== -->

</section>
