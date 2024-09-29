---
type: widget_page
---

<nav>
  <ul>
    <li><a href="?lang=en">English</a></li>
    <li><a href="?lang=ko">한국어</a></li>
  </ul>
</nav>

<div id="content">
  <p data-lang="en">Hello</p>
  <p data-lang="ko">안녕하세요</p>
</div>

<script>
  const userLang = new URLSearchParams(window.location.search).get('lang') || 'en';
  document.querySelectorAll('[data-lang]').forEach(el => {
    el.style.display = el.getAttribute('data-lang') === userLang ? 'block' : 'none';
  });
</script>
