---
layout: default
title: Research
permalink: /research/
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">RESEARCH OVERVIEW</p>
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
      <h3><a href="Enteric Nervous System and the Gut-Brain Axis/">Enteric Nervous System and the Gut-Brain Axis</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="Innate Sensing Understanding Host Responses to Gut Pathogens/">Innate Sensing: Understanding Host Responses to Gut Pathogens</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="Gastrointestinal Tumor Microenvironment and Metastasis/">Gastrointestinal Tumor Microenvironment and Metastasis</a></h3>
      <p>Click to view details</p>
    </article>
    <article class="stack-card">
      <h3><a href="Advancing Medical Science with Deep Gut Tissue Optogenetics/">Advancing Medical Science with Deep Gut Tissue Optogenetics</a></h3>
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
