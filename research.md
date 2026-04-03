---
layout: default
title: Research
permalink: /research/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">HIGHLIGHT</p>
    </div>
  </div>
  <div class="image-panel publication-feature-figure">
    <img src="{{ '/assets/images/publication-flowchart.jpg' | relative_url }}" alt="Research overview flowchart">
  </div>
</section>

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">RESEARCH PROJECTS</p>
    </div>
  </div>
  <div class="stack-list">
    <article class="stack-card">
      <h3><a href="/research/project-1/">PROJECT 1</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="/research/project-2/">PROJECT 2</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="/research/project-3/">PROJECT 3</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="/research/project-4/">PROJECT 4</a></h3>
      <p>Click to view details</p>
    </article>
  </div>
</section>

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">RESEARCH OVERVIEW</p>
    </div>
  </div>
  <div class="stack-list">
    {% for item in site.data.research %}
      <article class="stack-card">
        <h3>{{ item.title | upcase }}</h3>
        <p>{{ item.summary }}</p>
        <ul>
          {% for bullet in item.bullets %}
            <li>{{ bullet }}</li>
          {% endfor %}
        </ul>
      </article>
    {% endfor %}
  </div>
</section>
