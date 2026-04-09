<header class="site-header">
  <div class="container header-inner">
    <a class="brand brand-wordmark-image" href="{{ '/' | relative_url }}">
      <img src="{{ '/assets/images/tanlab-logo9.png' | relative_url }}" alt="Tan Lab">
    </a>

    <button class="menu-toggle" type="button" aria-label="Toggle navigation" onclick="document.body.classList.toggle('nav-open')">
      ☰
    </button>

    <nav class="site-nav">
      <a href="{{ '/' | relative_url }}"{% if page.url == '/' %} class="active"{% endif %}>HOME</a>
      <a href="{{ '/team/' | relative_url }}"{% if page.url == '/team/' %} class="active"{% endif %}>TEAM</a>
      <a href="{{ '/research/' | relative_url }}"{% if page.url == '/research/' %} class="active"{% endif %}>RESEARCH</a>
      <a href="{{ '/publications/' | relative_url }}"{% if page.url == '/publications/' %} class="active"{% endif %}>PUBLICATIONS</a>
      <a href="{{ '/seminar/' | relative_url }}"{% if page.url == '/seminar/' %} class="active"{% endif %}>LAB SEMINAR</a>
      <a href="{{ '/news/' | relative_url }}"{% if page.url == '/news/' %} class="active"{% endif %}>NEWS</a>
      <a href="{{ '/lab-gallery/' | relative_url }}"{% if page.url == '/lab-gallery/' %} class="active"{% endif %}>GALLERY</a>
      <a href="{{ '/resources/' | relative_url }}"{% if page.url == '/resources/' %} class="active"{% endif %}>RESOURCES</a>
      <a href="{{ '/contact/' | relative_url }}"{% if page.url == '/contact/' %} class="active"{% endif %}>CONTACT</a>
    </nav>
  </div>
</header>

<style>
/* 让头部和页面内容完全对齐（不超出） */
.site-header .container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  width: 100%;
  box-sizing: border-box;
}

/* 加高头部高度，更舒服 */
.site-header {
  padding: 20px 0;
}

/* 布局正常 */
.header-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* ✅ 这里是关键：tab 间距直接拉大！ */
.site-nav {
  display: flex;
  gap: 28px; /* 间距拉大，想更大就改 32px / 35px */
  flex-wrap: nowrap;
  justify-content: flex-end;
}

/* 文字不换行 */
.site-nav a {
  white-space: nowrap;
  text-decoration: none;
  font-size: 15px;
}

/* 移动端正常 */
@media (max-width: 768px) {
  .site-nav { display: none; }
  .nav-open .site-nav {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 80px;
    left: 0;
    right: 0;
    background: white;
    padding: 20px;
    gap: 15px;
  }
}
</style>
