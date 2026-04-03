---
layout: default
title: Home
---

<section class="hero hero-home">
  <div class="hero-visual image-panel">
    <img src="{{ site.data.site.home_hero_image }}" alt="Tan Lab home image">
  </div>

  <div class="hero-copy">
    <h1 style="text-align: justify; font-size: 1.1rem; line-height: 1.6; font-weight: normal;">
      {{ site.data.site.intro }}
    </h1>
    <div class="cta-row">
      <a class="button" href="{{ '/research/' | relative_url }}">Explore Research</a>
      <a class="button secondary" href="{{ '/publications/' | relative_url }}">View Publications</a>
    </div>
  </div>
</section>

<section class="section">
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
