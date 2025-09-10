<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="utf-8" />
  <title>Професійна установка та чистка кондиціонерів — Анатолій</title>
  <!-- Фіксований масштаб: забороняємо зум -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no" />
  <meta name="format-detection" content="telephone=no" />
  <meta name="theme-color" content="#ff8a1f" />

  <style>
    /* Базові налаштування */
    *, *::before, *::after { box-sizing: border-box; }
    html, body { height: 100%; }
    html { -webkit-text-size-adjust: 100%; }
    body {
      margin: 0;
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, "Helvetica Neue", Arial, "Noto Sans", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
      color: #fff;
      line-height: 1.45;
      background: #111;
      overflow-x: hidden;
      touch-action: manipulation;           /* прибирає подвійний тап зум */
      overscroll-behavior: none;            /* без "пружини" на iOS */
    }

    /* Фонова картинка з мінімальним блюром + затемненням для читабельності */
    .bg {
      position: fixed;
      inset: 0;
      z-index: -2;
    }
    .bg::before {
      content: "";
      position: absolute;
      inset: 0;
      background-image: url("https://i.ibb.co/gFftbdMm/402aca30-0c83-41a0-b7a1-bbec39950726.png");
      background-size: cover;
      background-position: center;
      filter: blur(1.5px); /* мінімальний розмив */
      transform: scale(1.02); /* щоб краї блюра не темніли */
    }
    .bg::after {
      content: "";
      position: absolute;
      inset: 0;
      background: radial-gradient(1200px 700px at 70% 20%, rgba(0,0,0,0.15), rgba(0,0,0,0.58)),
                  linear-gradient(180deg, rgba(0,0,0,0.45), rgba(0,0,0,0.70));
      z-index: -1;
    }

    /* Контейнер */
    .wrap {
      max-width: 1100px;
      margin: 0 auto;
      padding: 22px clamp(14px, 3.2vw, 28px) 48px;
    }

    /* Шапка */
    .topbar {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 12px;
      padding: 8px 0 16px;
    }
    .brand {
      display: flex;
      align-items: center;
      gap: 10px;
      font-weight: 800;
      letter-spacing: .4px;
      text-transform: uppercase;
      font-size: clamp(18px, 2.6vw, 28px);
      line-height: 1.1;
    }
    .brand .dot {
      width: 12px; height: 12px; border-radius: 50%;
      background: #ff8a1f;
      box-shadow: 0 0 0 6px rgba(255,138,31,0.2);
    }
    .cta-top {
      display: flex; gap: 10px; flex-wrap: wrap;
    }
    .btn {
      appearance: none; border: 0; cursor: pointer;
      padding: 12px 18px; border-radius: 12px;
      font-weight: 700; text-decoration: none; color: #141414;
      background: linear-gradient(180deg, #ff9b3b, #ff8a1f);
      box-shadow: 0 6px 18px rgba(255,138,31,.35), inset 0 1px 0 rgba(255,255,255,.35);
      transition: transform .08s ease-in-out, box-shadow .12s ease-in-out, opacity .2s;
      white-space: nowrap;
    }
    .btn:active { transform: translateY(1px) scale(.99); }
    .btn--ghost {
      background: rgba(255,255,255,.08);
      color: #fff; box-shadow: inset 0 0 0 1px rgba(255,255,255,.2);
    }

    /* Хедлайн-блок */
    .hero {
      display: grid;
      grid-template-columns: 1fr;
      gap: 22px;
      padding: 8px 0 10px;
    }
    .badge {
      display: inline-flex; align-items: center; gap: 10px;
      background: rgba(255,138,31,.95);
      color: #1b0a00; font-weight: 800;
      border-radius: 16px; padding: 10px 14px;
      width: max-content;
      box-shadow: 0 10px 22px rgba(255,138,31,.35);
      letter-spacing: .2px;
    }
    .hero h1 {
      margin: 0;
      font-size: clamp(28px, 6.2vw, 54px);
      line-height: 1.05;
      font-weight: 900;
      text-transform: uppercase;
      text-wrap: balance;
    }
    .hero p {
      margin: 0;
      font-size: clamp(15px, 2.4vw, 18px);
      color: #eaeaea;
      max-width: 880px;
    }

    /* Карточки послуг */
    .cards {
      display: grid;
      grid-template-columns: repeat(12, 1fr);
      gap: 16px;
      margin-top: 18px;
    }
    .card {
      grid-column: span 12;
      background: rgba(24, 24, 24, 0.72);
      backdrop-filter: saturate(120%) blur(2px);
      border-radius: 18px;
      padding: clamp(16px, 3vw, 24px);
      box-shadow: 0 14px 28px rgba(0,0,0,.35), inset 0 0 0 1px rgba(255,255,255,.06);
    }
    .card h3 {
      margin: 0 0 10px 0;
      font-size: clamp(20px, 3.4vw, 28px);
      line-height: 1.15;
    }
    .grid-6 { grid-column: span 12; }
    @media (min-width: 860px) {
      .grid-6 { grid-column: span 6; }
    }

    .checklist { list-style: none; padding: 0; margin: 12px 0 0 0; display: grid; gap: 10px; }
    .li {
      display: grid; grid-template-columns: 24px 1fr; gap: 10px; align-items: start;
      font-size: clamp(15px, 2.3vw, 18px);
      color: #f2f2f2;
    }
    .ico {
      width: 22px; height: 22px; flex: 0 0 22px;
      border-radius: 6px;
      background: linear-gradient(180deg, #ff9b3b, #ff8a1f);
      display: grid; place-items: center;
      box-shadow: 0 4px 10px rgba(255,138,31,.35);
    }
    .ico svg { width: 16px; height: 16px; fill: #1b0a00; }

    /* Прайс-блок */
    .price {
      display: flex; align-items: center; gap: 12px; flex-wrap: wrap;
      margin-top: 6px;
    }
    .pill {
      display: inline-flex; align-items: center; gap: 10px;
      padding: 8px 12px; border-radius: 999px;
      background: rgba(255,255,255,.08);
      border: 1px solid rgba(255,255,255,.14);
      color: #fff;
      font-weight: 700;
    }
    .tag-off { background: linear-gradient(180deg, #ff9b3b, #ff8a1f); color: #1b0a00; border: 0; }
    .price-big {
      font-size: clamp(26px, 5.2vw, 40px); font-weight: 900; letter-spacing: 0.4px;
    }
    .price-old {
      text-decoration: line-through; opacity: .7; font-weight: 700;
      font-size: clamp(16px, 3.2vw, 20px);
    }

    /* Контакти */
    .contact {
      display: grid; gap: 10px;
      margin-top: 18px;
      font-size: clamp(15px, 2.4vw, 18px);
    }
    .phone {
      font-weight: 900; font-size: clamp(20px, 3.8vw, 28px);
      letter-spacing: .3px;
    }
    .contact .row { display: flex; gap: 10px; flex-wrap: wrap; align-items: center; }
    .a-lite { color: #fff; text-decoration: none; border-bottom: 1px dashed rgba(255,255,255,.35); }
    .a-lite:hover { opacity: .9; }

    /* Нижній банер-гарантія */
    .guarantee {
      margin-top: 18px;
      background: linear-gradient(180deg, rgba(255,138,31,.18), rgba(255,138,31,.28));
      border: 1px solid rgba(255,138,31,.45);
      color: #fff;
      padding: clamp(14px, 3vw, 18px);
      border-radius: 14px;
      box-shadow: inset 0 0 30px rgba(255,138,31,.12);
      font-weight: 700;
      text-align: center;
    }

    /* Футер */
    footer {
      opacity: .9;
      font-size: 13px;
      text-align: center;
      padding-top: 24px;
    }

    /* Безпечна зона для кнопок на айфонах */
    .safe-bottom { height: env(safe-area-inset-bottom); }

  </style>
</head>
<body>
  <!-- Фон -->
  <div class="bg" aria-hidden="true"></div>

  <!-- Контент -->
  <div class="wrap">
    <header class="topbar">
      <div class="brand"><span class="dot"></span> Кондиціонери • Одеса</div>
      <div class="cta-top">
        <a class="btn" href="tel:+380958355990" aria-label="Подзвонити Анатолію">📞 Подзвонити</a>
        <a class="btn btn--ghost" href="viber://chat?number=%2B380958355990" aria-label="Написати у Viber">Viber</a>
        <a class="btn btn--ghost" href="https://t.me/" target="_blank" rel="noopener" aria-label="Написати у Telegram">Telegram</a>
      </div>
    </header>

    <section class="hero">
      <span class="badge">Гарантія 12 місяців</span>
      <h1>Професійна установка, чистка, сервіс і продаж кондиціонерів</h1>
      <p>
        🔧 Чистий кондиціонер — свіже повітря у вашій оселі! Працюємо швидко, акуратно і з гарантією.
        Обслуговуємо квартири, офіси та комерційні приміщення. Одеса та Одеська область.
      </p>
      <div class="cta-top" style="margin-top:6px">
        <a class="btn" href="tel:+380958355990">Замовити зараз</a>
        <a class="btn btn--ghost" href="#services">Дізнатися деталі</a>
      </div>
    </section>

    <section id="services" class="cards">

      <!-- УСТАНОВКА -->
      <article class="card grid-6">
        <h3>Професійна установка кондиціонеру</h3>
        <ul class="checklist">
          <li class="li">
            <span class="ico" aria-hidden="true">
              <svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg>
            </span>
            <span>Акуратне встановлення внутрішнього та зовнішнього блоку</span>
          </li>
          <li class="li">
            <span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Оптимальна прокладка комунікацій</span>
          </li>
          <li class="li">
            <span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Підключення та перевірка роботи системи</span>
          </li>
          <li class="li">
            <span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Заправка фреоном — за потреби</span>
          </li>
        </ul>
        <div class="contact">
          <div class="row"><strong>Анатолій</strong></div>
          <div class="row phone">+38 (095) 835 59 90</div>
          <div class="row">
            <a class="btn" href="tel:+380958355990">Замовити установку</a>
            <a class="btn btn--ghost" href="viber://chat?number=%2B380958355990">Написати у Viber</a>
          </div>
        </div>
      </article>

      <!-- ЧИСТКА -->
      <article class="card grid-6">
        <h3>Чистка кондиціонеру <span class="pill tag-off">−25%</span></h3>

        <div class="price">
          <div class="price-big">1200 грн</div>
          <div class="price-old">1500</div>
        </div>

        <ul class="checklist" style="margin-top:12px">
          <li class="li"><span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Розбирання та чистка фільтрів</span></li>
          <li class="li"><span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Видалення пилу, бруду та цвілі</span></li>
          <li class="li"><span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Дезінфекція від бактерій і грибків</span></li>
          <li class="li"><span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Промивання дренажної системи</span></li>
          <li class="li"><span class="ico"><svg viewBox="0 0 24 24"><path d="M9 16.2l-3.5-3.5-1.4 1.4L9 19 20.3 7.7l-1.4-1.4z"/></svg></span>
            <span>Перевірка роботи кондиціонера</span></li>
        </ul>

        <div class="contact">
          <div class="row"><strong>Анатолій</strong></div>
          <div class="row phone">+38 (095) 835 59 90</div>
          <div class="row">
            <a class="btn" href="tel:+380958355990">Замовити чистку</a>
            <a class="btn btn--ghost" href="https://t.me/" target="_blank" rel="noopener">Написати у Telegram</a>
          </div>
        </div>
      </article>

      <!-- ДОДАТКОВО: продаж та підбір -->
      <article class="card" style="grid-column: span 12;">
        <h3>Продаж і професійна установка «під ключ»</h3>
        <p style="margin:8px 0 0 0; color:#f3f3f3">
          🆕 Підберемо оптимальний кондиціонер під площу вашого приміщення, доставимо, встановимо і дамо гарантію.
          💨 Замовляйте чистку, установку чи заправку — дихайте на повні груди!
        </p>
        <div class="contact" style="margin-top:12px">
          <div class="row">
            <span class="pill">Одеса та Одеська область</span>
            <span class="pill">Швидко • Акуратно • З гарантією</span>
          </div>
          <div class="row">
            <a class="btn" href="tel:+380958355990">Зв’язатися</a>
            <a class="btn btn--ghost" href="viber://chat?number=%2B380958355990">Viber</a>
            <a class="btn btn--ghost" href="https://t.me/" target="_blank" rel="noopener">Telegram</a>
          </div>
        </div>
      </article>

    </section>

    <div class="guarantee">
      Гарантуємо акуратність, швидкість і довговічність результату. Працюємо офіційно, надаємо чек та гарантію 12 місяців.
    </div>

    <footer>
      © <span id="y"></span> Анатолій • Кондиціонери • Одеса / Одеська область
      <div class="safe-bottom"></div>
    </footer>
  </div>

  <script>
    // Підстановка поточного року у футері
    document.getElementById('y').textContent = new Date().getFullYear();

    // Додатковий захист від зуму (iOS подвійний тап / pinch)
    (function () {
      let lastTouchEnd = 0;
      document.addEventListener('touchend', function (e) {
        const now = Date.now();
        if (now - lastTouchEnd <= 350) { e.preventDefault(); }
        lastTouchEnd = now;
      }, { passive: false });

      document.addEventListener('gesturestart', function (e) { e.preventDefault(); }, { passive: false });
      document.addEventListener('gesturechange', function (e) { e.preventDefault(); }, { passive: false });
      document.addEventListener('gestureend', function (e) { e.preventDefault(); }, { passive: false });
    })();
  </script>
</body>
</html>
