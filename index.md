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
/* 全局头部样式：全站所有页面生效 */
.site-header {
  padding: 20px 0;
  background: #fff;
}
.site-header .container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  width: 100%;
  box-sizing: border-box;
}
.header-inner {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

/* 桌面端导航：不换行、不超出、间距适中 */
.site-nav {
  display: flex;
  gap: 18px;
  flex-wrap: nowrap;
  justify-content: flex-end;
}
.site-nav a {
  white-space: nowrap;
  font-size: 15px;
  text-decoration: none;
}

/* 🔥 手机版菜单：完美不挤、竖排显示 */
@media (max-width: 768px) {
  .menu-toggle {
    display: block !important;
    background: none;
    border: none;
    font-size: 24px;
    cursor: pointer;
  }
  .site-nav {
    display: none;
  }
  .nav-open .site-nav {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 70px;
    left: 0;
    right: 0;
    background: #fff;
    padding: 20px;
    gap: 16px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    z-index: 999;
  }
}
</style>
