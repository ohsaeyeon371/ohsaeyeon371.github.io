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
  <p data-lang="en">Hi, there! I'm Alice, a machine learning researcher at Netflix.</p>
  <p data-lang="ko">안녕하세요! 저는 Netflix에서 기계 학습 연구원으로 일하는 Alice입니다.</p>
</div>

<script>
  const userLang = new URLSearchParams(window.location.search).get('lang') || 'en';
  document.querySelectorAll('[data-lang]').forEach(el => {
    el.style.display = el.getAttribute('data-lang') === userLang ? 'block' : 'none';
  });
</script>
