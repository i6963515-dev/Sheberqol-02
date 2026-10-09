<!doctype html>
<html lang="kk">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#000000">
  <meta name="description" content="ШеберҚол — қолөнер шеберлерінің бұйымдар каталогы">
  <title>ШеберҚол — қолөнер маркетплейсі</title>
  <link rel="icon" href="assets/favicon.png">
  <link rel="stylesheet" href="style.css">
</head>
<body class="high-contrast">
  <header class="topbar">
    <a class="brand" href="#" aria-label="ШеберҚол басты бет"><span class="brand-icon">◉</span><span>ШеберҚол</span></a>
    <div class="accessibility-controls">
      <button class="icon-button" id="speechToggle" aria-label="Экрандық оқырманды қосу/өшіру" title="Дыбыстау"><span id="speechIcon">🔊</span></button>
      <button class="icon-button" id="contrastToggle" aria-label="Контраст режимін өзгерту" title="Контраст режимі"><span id="contrastIcon">◉</span></button>
    </div>
  </header>

  <nav class="tabs" aria-label="Негізгі бөлімдер">
    <button class="tab active" data-tab="marketplace"><span>🛍️</span> Каталог</button>
    <button class="tab" data-tab="ai-upload"><span>✨</span> Шебер ЖИ</button>
    <button class="tab" data-tab="tech-stack"><span>⌘</span> Стек</button>
  </nav>

  <main class="page-content">
    <section class="panel active" id="marketplace">
      <label class="search-box"><span aria-hidden="true">⌕</span><input id="searchInput" type="search" placeholder="Іздеу (киіз, ағаш)..." aria-label="Бұйымдарды іздеу"></label>
      <div id="productList" class="product-list" aria-live="polite"></div>
      <p class="empty-state" id="emptyState" hidden>Іздеу бойынша бұйым табылмады.</p>
    </section>

    <section class="panel" id="ai-upload" hidden>
      <article class="card">
        <h1>ЖИ Фото-Көмекші</h1>
        <p class="muted">Камера бұйымды түсіріп, сипаттамасын автоматты түрде дайындауға көмектеседі.</p>
        <div class="camera-box" id="cameraBox"><span class="camera-symbol">▣</span><p id="cameraStatus">Бұйымды жариялауды бастау үшін төмендегі батырманы басыңыз.</p></div>
        <button class="primary-button full-width" id="photoButton">📸 Бұйымды фотоға түсіру</button>
        <form id="publishForm" hidden>
          <label class="field-label" for="newTitle">Бұйым атауы:</label>
          <input class="field" id="newTitle" required value="Қолдан тігілген Былғары Торсық">
          <label class="field-label" for="newPrice">Бағасы (₸):</label>
          <input class="field" id="newPrice" type="number" min="0" value="18000" required>
          <p class="muted" id="aiDescription">Сипаттама дайын.</p>
          <button class="primary-button full-width" type="submit">Жариялау</button>
        </form>
      </article>
    </section>

    <section class="panel" id="tech-stack" hidden>
      <article class="card">
        <h1>IT Архитектура</h1>
        <div class="tech-item"><span>📱</span><p>1. HTML / CSS / JavaScript — веб-нұсқасы</p></div>
        <div class="tech-item"><span>🔊</span><p>2. Браузердің Speech Synthesis API — мәтінді дыбыстау</p></div>
        <div class="tech-item"><span>✨</span><p>3. ЖИ фото-көмекшісінің демонстрациялық үлгісі</p></div>
        <div class="tech-item"><span>🗃️</span><p>4. GitHub Pages арқылы жариялауға дайын статикалық сайт</p></div>
        <p class="muted">Ескерту: ЖИ талдауы мен Kaspi төлемі бұл нұсқада нақты сыртқы қызметтерге қосылмаған.</p>
      </article>
    </section>
  </main>
  <footer>© 2026 ШеберҚол · Қазақ қолөнерін қолдаймыз</footer>
  <script src="script.js"></script>
</body>
</html>
