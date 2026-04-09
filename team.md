---
layout: default
title: Team
permalink: /team/
---

<style>
.team-profile-block {
  margin: 0 0 28px;
}

.team-profile-card {
  display: flex;
  align-items: center;
  gap: 36px;
  padding: 8px 0 0;
}

.team-profile-side {
  flex: 0 0 240px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.team-profile-photo {
  width: 118px;
  height: 118px;
  border-radius: 0;
  overflow: hidden;
  background: #fff;
  margin: 0 0 16px;
}

.team-profile-photo img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.team-profile-side h3 {
  margin: 0 0 8px;
  font-size: 1rem;
  line-height: 1.32;
  letter-spacing: 0.01em;
  color: var(--ink);
}

.team-profile-role {
  margin: 0 0 6px;
  font-size: 0.86rem;
  line-height: 1.45;
  color: var(--ink);
  font-weight: 600;
}

.team-profile-meta {
  margin: 0;
  font-size: 0.82rem;
  line-height: 1.55;
  color: var(--ink);
}

.team-profile-copy {
  flex: 1;
  max-width: 760px;
  min-width: 0;
}

.team-profile-bio {
  margin: 0;
  font-size: 1rem;
  line-height: 1.55;
  color: var(--muted);
  text-align: justify;
}

.team-grid--members:empty::before {
  content: "";
  display: block;
  min-height: 12px;
}

.team-section--alumni .member-card .card-body {
  padding-top: 18px;
  padding-bottom: 18px;
}

.team-section--alumni .member-card .card-body h3 {
  margin: 0 0 6px;
  line-height: 1.08;
}

.team-section--alumni .member-card .card-body p,
.team-section--alumni .member-meta,
.team-section--alumni .member-link {
  margin: 0 0 2px;
  line-height: 1.08;
}

.team-section--alumni .member-card .card-body p:last-child,
.team-section--alumni .member-link:last-child {
  margin-bottom: 0;
}

@media (max-width: 980px) {
  .team-profile-card {
    flex-direction: column;
    gap: 26px;
  }

  .team-profile-side {
    flex-basis: auto;
    width: 100%;
  }

  .team-profile-photo {
    width: 118px;
    height: 118px;
  }

  .team-profile-copy {
    max-width: 100%;
  }
}
</style>

<!-- 全部内容放在同一个 section 框内 -->
<section class="section">

  <!-- PRINCIPAL INVESTIGATOR -->
  <div class="section-head">
    <div>
      <p class="eyebrow">PRINCIPAL INVESTIGATOR</p>
    </div>
  </div>

  {% assign lead = site.data.team | first %}
  <div class="team-profile-card">
    <div class="team-profile-side">
      <div class="team-profile-photo">
        <img src="/assets/images/peng-tan.png" alt="{{ lead.name }}" loading="lazy">
      </div>

      <h3>{{ lead.name }}</h3>
      <p class="team-profile-role">Principal Investigator</p>
      <p class="team-profile-meta">Hainan Medical University</p>
    </div>

    <div class="team-profile-copy">
      <p class="team-profile-bio">Peng Tan is a professor and principal investigator at Hainan Academy of Medical Sciences, Hainan Medical University. He earned his Ph.D. from Texas A&M University in 2018 and conducted off-campus research at the Weill Cornell Medical College-Houston campus. He then joined the Klarman Cell Observatory at the Broad Institute and MIT HHMI as a postdoctoral associate under Professors Aviv Regev and Ramnik Xavier. As a team member of the Food Allergy Science Initiative and the Human Cell Atlas, he contributed extensively to high-impact publications across Nature, Nature Medicine, Nature Cell Biology, Cell Host & Microbe, and Immunity. He is the recipient of the Student Research Award and the IBD Plexus Award from the Crohn's & Colitis Foundation of America. He has published over 40 peer-reviewed papers, including first and corresponding author articles in leading journals such as Science, Nature Chemical Biology, Physiological Reviews, Nucleic Acids Research, Molecular Cell, and the Journal of Clinical Investigation. His work has accumulated more than 4,250 citations and an h-index of 29, and has been featured and highlighted in multiple academic journals and media outlets.</p>
    </div>
  </div>


  <!-- LAB MEMBERS -->
  <div class="section-head" style="margin-top: 48px;">
    <div>
      <p class="eyebrow">LAB MEMBERS</p>
    </div>
  </div>

  <!-- 合照（缩小 + 居中） -->
  <div style="margin-top: 12px; margin-bottom: 32px; text-align: center;">
    <img src="/assets/images/team-photo.png?v=3"
         style="max-width: 720px; width: 85%; border-radius: 16px; object-fit: cover;"
         alt="Lab Members">
  </div>

  <!-- 成员列表 -->
  <div style="padding: 0 0 12px;">
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Wanrong Xia</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Administrative assistant</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Jiaxing Wang</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Ph.D student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Wen Jiang</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Ph.D student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Jinyi Xiang</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Master's student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Xinyu Zhang</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Master's student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Zeyan Han</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Master's student-Computation</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Ting Wei</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Master's student-Computation</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Zixuan Song</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Yihan Du</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Weiyuan Ding</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Arun Dong</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Lingfei Liu</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Yidan Zhao</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">Wanxiang Shi</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">Undergraduate student</span>
    </div>
  </div>


  <!-- Former members -->
  <div class="section-head" style="margin-top: 48px;">
    <div>
      <p class="eyebrow">FORMER MEMBERS</p>
    </div>
  </div>

  <div style="padding: 0 0 12px;">
    {% for member in site.data.team offset:1 %}
    <div style="padding: 6px 0; font-size: 0.94rem; border-bottom: 1px solid var(--line);">
      <span style="font-weight: 600; color: var(--ink);">{{ member.name }}</span>
      <span style="margin: 0 10px; color: var(--muted);">–</span>
      <span style="color: var(--muted);">{{ member.role }}</span>
      {% if member.link %}
      <span style="margin: 0 10px; color: var(--muted);">|</span>
      <a href="{{ member.link }}" target="_blank" rel="noopener noreferrer" style="color: var(--accent);">
        {{ member.link }}
      </a>
      {% endif %}
    </div>
    {% endfor %}
  </div>

</section>
