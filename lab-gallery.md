---
layout: default
title: Gallery
permalink: /lab-gallery/
---

<section class="page-hero page-hero--compact">
  <p class="eyebrow">GALLERY</p>
</section>

<section class="section">
  <div class="gallery-grid">

    <!-- 照片 1 -->
    <div class="gallery-item">
      <img src="/assets/images/team-photo-yikeyuan.jpg" alt="Gallery photo">
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-23</span>
        <p>Group photo at Hainan Academy of Medical Sciences</p>
      </div>
    </div>

    <!-- 照片 2 -->
    <div class="gallery-item">
      <img src="/assets/images/team-photo-huoshankou.jpg" alt="Gallery photo">
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at Leiqiong UNESCO Global Geopark</p>
      </div>
    </div>

    <!-- 照片 3 -->
    <div class="gallery-item">
      <img src="/assets/images/team-photo-huoshankou2.jpg" alt="Gallery photo">
      <div class="gallery-caption">
        <span class="gallery-date">2026-01-30</span>
        <p>Tan lab retreat at Leiqiong UNESCO Global Geopark</p>
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
}

.gallery-item img {
  width: 100%;
  height: 220px;
  object-fit: cover;
  display: block;
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
