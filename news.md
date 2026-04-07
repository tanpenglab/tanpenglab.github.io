---
layout: default
---

<section class="section">
  <div class="section-head">
    <div>
      <p class="eyebrow">LAB NEWS</p>
    </div>
  </div>

  <!-- 整个帖子统一一个框 -->
  <div style="
    border: 1px solid #e5e7eb;
    border-radius: 14px;
    padding: 30px 32px;
    background: #ffffff;
    max-width: 800px;
    margin: 0 auto;
  ">
    <h1 style="
      margin: 0 0 20px;
      font-size: 1.4rem;
      font-weight: 700;
      line-height: 1.4;
      color: var(--ink);
    ">{{ page.title }}</h1>

    <div style="
      font-size: 1rem;
      line-height: 1.7;
      color: var(--ink);
    ">
      {{ content }}
    </div>
  </div>
</section>
