---
layout: default
title: Gallery
permalink: /lab-gallery/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB GALLERY</p>
    </div>
  </div>

  <div class="gallery-grid">

    <!-- 照片 1 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/team-photo-yikeyuan.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-23</span>
        <p>Group photo at Hainan Academy of Medical Sciences</p>
      </div>
    </div>

    <!-- 照片 2 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/team-photo-huoshankou.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at Leiqiong UNESCO Global Geopark</p>
      </div>
    </div>

    <!-- 照片 3 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/team-photo-huoshankou2.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at Leiqiong UNESCO Global Geopark</p>
      </div>
    </div>

    <!-- 照片 4 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-0.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣堂村</p>
      </div>
    </div>

    <!-- 照片 5 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-1.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣山寮</p>
      </div>
    </div>

    <!-- 照片 6 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-2.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣山寮</p>
      </div>
    </div>

    <!-- 照片 7 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-3.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣山寮</p>
      </div>
    </div>

    <!-- 照片 8 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-4.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣山寮</p>
      </div>
    </div>

    <!-- 照片 9 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/20260130retreat-5.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at 荣山寮</p>
      </div>
    </div>
    
    <!-- 照片 10 -->
    <div class="gallery-item">
      <div class="gallery-img-wrap">
        <img src="/assets/images/team-photo yikeyuan.jpg" alt="Gallery photo">
      </div>
      <div class="gallery-caption">
        <span class="gallery-date">2026-07-17</span>
        <p>Group photo at Hainan Academy of Medical Sciences</p>
      </div>
    </div>

  </div>
</section>

<style>
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 24px;
  margin-top: 12px;
}

.gallery-item {
  background: #fff;
  border-radius: 16px;
  overflow: hidden;
  box-shadow: var(--shadow);
  display: flex;
  flex-direction: column;
}

/* 统一图片容器比例 4:3，可以自行修改 */
.gallery-img-wrap {
  width: 100%;
  height: 240px;
  background-color: #f6f6f6;
  display: flex;
  align-items: center;
  justify-content: center;
}

.gallery-img-wrap img {
  max-width: 100%;
  max-height: 100%;
  display: block;
  object-fit: contain;
}

.gallery-caption {
  padding: 14px 16px;
}

.gallery-date {
  font-size: 0.85rem;
  color: var(--accent);
  font-weight: 600;
  display: block;
  margin-bottom: 4px;
}

.gallery-caption p {
  margin: 0;
  font-size: 0.9rem;
  color: var(--ink);
  line-height: 1.5;
}
</style>
