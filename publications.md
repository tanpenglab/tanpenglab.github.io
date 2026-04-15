---
layout: default
title: Publications
permalink: /publications/
---

<style>
.pub-list .pub-gallery {
  display: none;
}

.pub-list .pub-gallery.pub-gallery--show {
  display: flex !important;
  margin-top: 18px;
}

.pub-list .pub-gallery.pub-gallery--featured {
  display: flex !important;
  width: 100%;
  justify-content: center;
}

.pub-list .pub-gallery.pub-gallery--featured img {
  width: 66.666%;
  max-width: 66.666%;
  max-height: none;
  display: block;
  margin: 0 auto;
}
</style>

<!-- 所有内容放在同一个 section 框内 -->
<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">PUBLICATIONS</p>
      <!-- Google Scholar 放在这里 -->
      <div class="scholar-row" style="margin: 8px 0 0 0;">
        <a href="https://scholar.google.com/citations?user=i6kV0H8AAAAJ&hl=en&oi=ao" target="_blank" rel="noopener noreferrer">
          <img src="{{ site.data.site.publications_scholar_image }}" alt="Google Scholar">
        </a>
      </div>
      <p style="margin: 12px 0 0 0;"># denotes co-first authors; * denotes corresponding authors</p>
    </div>
  </div>

  <!-- ARTICLES -->
  <div class="section-head" style="margin-top: 48px;">
    <div>
      <p class="eyebrow">ARTICLES</p>
    </div>
  </div>

  <div class="pub-list">
    {% for item in site.data.publications %}
      <article class="pub-item">
        <div class="pub-meta">
          <span class="pub-journal">{{ item.journal }}</span>
          <span>•</span>
          <span class="pub-date">{{ item.date }}</span>
        </div>
        <div class="pub-title">
          {% if item.url == '#' %}
            {{ item.title }}
          {% else %}
            <a href="{{ item.url }}" target="_blank" rel="noopener noreferrer">{{ item.title }}</a>
          {% endif %}
        </div>
        <div>{{ item.authors | raw }}</div>
        {% if item.note %}<div class="note">{{ item.note }}</div>{% endif %}

        {% if item.images %}
          {% capture article_image_index %}{% increment article_image_count %}{% endcapture %}
          {% assign article_image_index_num = article_image_index | plus: 0 %}
          {% assign hide_this_image = false %}
          {% if item.journal == 'Nucleic Acids Research' or item.journal == 'Advanced Biology' %}
            {% assign hide_this_image = true %}
          {% endif %}
          {% if article_image_index_num < 4 and hide_this_image == false %}
            <div class="pub-gallery pub-gallery--show{% if article_image_index_num == 0 %} pub-gallery--featured{% endif %}">
              {% for img in item.images %}
                <img src="{{ img | relative_url }}" alt="{{ item.title }} figure {{ forloop.index }}">
              {% endfor %}
            </div>
          {% endif %}
        {% endif %}
      </article>
    {% endfor %}
  </div>

  <!-- REVIEWS -->
  <div class="section-head" style="margin-top: 48px;">
    <div>
      <p class="eyebrow">REVIEWS & BOOK CHAPTERS</p>
    </div>
  </div>

  <div class="review-list">
    {% for item in site.data.reviews %}
      <article class="pub-item">
        <div class="pub-meta">
          <span class="pub-journal">{{ item.journal }}</span>
          <span>•</span>
          <span class="pub-date">{{ item.date }}</span>
        </div>
        <div class="pub-title">
          <a href="{{ item.url }}" target="_blank" rel="noopener noreferrer">{{ item.title }}</a>
        </div>
        <div>{{ item.authors | raw }}</div>
        {% if item.note %}<div class="note">{{ item.note }}</div>{% endif %}
        {% if item.images %}
          <div class="pub-gallery">
            {% for img in item.images %}
              <img src="{{ img | relative_url }}" alt="{{ item.title }} figure {{ forloop.index }}">
            {% endfor %}
          </div>
        {% endif %}
      </article>
    {% endfor %}
  </div>
</section>
