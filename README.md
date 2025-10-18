[index.html](https://github.com/user-attachments/files/22987162/index.html)
<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Big0Soft — حلول برمجية متكاملة</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --primary:#1d3557; /* default palette — يمكنك تغييره */
      --accent:#457b9d;
      --muted:#6b7280;
      --bg:#f8fafc;
      --card:#ffffff;
      --radius:14px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;font-family:'Cairo',sans-serif;background:var(--bg);color:#111;line-height:1.5;
      -webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;
    }
    header{background:linear-gradient(90deg,var(--primary),var(--accent));color:#fff;padding:48px 20px 64px}
    .container{max-width:1100px;margin:0 auto;padding:0 20px}
    .top{display:flex;gap:20px;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:56px;height:56px;border-radius:12px;background:rgba(255,255,255,0.12);display:flex;align-items:center;justify-content:center;font-weight:700}
    .brand h1{margin:0;font-size:20px}
    nav{display:flex;gap:18px;align-items:center}
    nav a{color:rgba(255,255,255,0.95);text-decoration:none;font-weight:600}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:30px;align-items:center;margin-top:28px}
    .hero .copy h2{font-size:32px;margin:0 0 12px}
    .hero .copy p{color:rgba(255,255,255,0.95);margin:0 0 18px}
    .cta-group{display:flex;gap:12px;flex-wrap:wrap}
    .btn{display:inline-flex;align-items:center;gap:10px;padding:12px 18px;border-radius:10px;text-decoration:none;font-weight:700;cursor:pointer}
    .btn-whatsapp{background:#25D366;color:#fff}
    .btn-mail{background:rgba(255,255,255,0.12);color:#fff;border:1px solid rgba(255,255,255,0.14)}

    .hero-card{background:var(--card);border-radius:12px;padding:18px;box-shadow:0 10px 30px rgba(13,38,63,0.12);color:#111}
    .hero-card h4{margin:0 0 8px}
    .meta{display:flex;gap:12px;flex-wrap:wrap;margin-top:10px}
    .meta span{background:#f1f5f9;padding:8px 10px;border-radius:8px;font-weight:600;color:var(--muted)}

    main{padding:40px 0}
    .section{background:transparent;padding:28px 0}
    .card{background:var(--card);border-radius:12px;padding:20px;box-shadow:0 6px 18px rgba(12,38,63,0.06)}

    /* الخدمات */
    .services{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:18px}
    .service{padding:18px;border-radius:12px}
    .service h3{margin:0 0 8px}

    /* مميزات */
    .features{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .feature{display:flex;gap:12px;align-items:flex-start;padding:14px;border-radius:10px;background:#fff}
    .feature .dot{width:44px;height:44px;border-radius:8px;background:linear-gradient(180deg,var(--primary),var(--accent));color:#fff;display:flex;align-items:center;justify-content:center;font-weight:700}

    /* أعمالنا */
    .works{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:14px}
    .work{height:160px;border-radius:10px;background:linear-gradient(135deg,#eef2ff,#f8fafc);display:flex;align-items:center;justify-content:center;color:var(--muted);font-weight:700}

    /* Testimonials */
    .testimonials{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:14px}
    .test{padding:14px;border-radius:12px;background:#fff}

    /* Contact */
    .contact-grid{display:grid;grid-template-columns:1fr 360px;gap:20px}
    form input,form textarea{width:100%;padding:10px;border:1px solid #e6edf3;border-radius:8px;margin-bottom:10px;font-size:14px}
    form button{background:var(--primary);color:#fff;padding:12px 16px;border-radius:10px;border:0;font-weight:700;cursor:pointer}

    footer{padding:28px 0;background:transparent}
    .footer-inner{display:flex;gap:20px;align-items:center;justify-content:space-between}
    .small{color:var(--muted);font-size:13px}

    /* WhatsApp floating */
    .whatsapp-fab{position:fixed;bottom:22px;left:22px;background:#25D366;color:#fff;border-radius:999px;padding:12px 16px;box-shadow:0 8px 26px rgba(37,211,102,0.18);z-index:1000;display:flex;align-items:center;gap:8px;text-decoration:none;font-weight:700}

    /* responsive */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .contact-grid{grid-template-columns:1fr}
      .top{flex-direction:column;align-items:flex-start}
      .brand h1{font-size:18px}
      .hero .copy h2{font-size:26px}
    }

    @media (max-width:520px){
      header{padding:28px 14px}
      .logo{width:48px;height:48px}
      .hero .copy h2{font-size:22px}
    }
  </style>
</head>
<body>
  <header>
    <div class="container">
      <div class="top">
        <div class="brand">
         <img src="assets/logo.png" alt="Big0Soft Logo" class="logo-img" style="width:60px;height:auto;border-radius:12px;" />

          <div>
            <h1>Big0Soft</h1>
            <div style="color:rgba(255,255,255,0.9);font-size:13px;margin-top:4px">حلول برمجية متكاملة — مواقع، تطبيقات، أنظمة</div>
          </div>
        </div>
        <nav>
          <a href="#services">خدماتنا</a>
          <a href="#works">أعمالنا</a>
          <a href="#contact">تواصل</a>
        </nav>
      </div>

      <div class="hero">
        <div class="copy">
          <h2>نحو تجربة رقمية أقوى لشركتك</h2>
          <p>نقوم بتصميم وتطوير مواقع احترافية وتطبيقات موبايل مخصصة تساعد نشاطك التجاري على النمو وتسريع الأعمال.</p>
          <div class="cta-group">
            <!-- Replace PHONE_NUMBER with your full international phone (no plus sign). Example: 962791234567 -->
            <a class="btn btn-whatsapp" href="https://wa.me/0000000000?text=مرحبًا%20Big0Soft!%20أرغب%20بخدمة%20" target="_blank" rel="noopener" aria-label="تواصل عبر واتساب">📱 تواصل عبر واتساب</a>
            <a class="btn btn-mail" href="https://mail.google.com/mail/?view=cm&fs=1&to=ahmadayad0@gmail.com" target="_blank" rel="noopener" aria-label="ارسال ايميل">✉️ راسلنا عبر الجيميل</a>
          </div>

          <div style="margin-top:16px;color:rgba(255,255,255,0.92);font-weight:600">خدماتنا الرئيسية: تصميم مواقع • تطبيقات موبايل • حلول مخصصة</div>
        </div>

        <div class="hero-card card">
          <h4>احجز استشارة مجانية</h4>
          <p style="margin:6px 0 0;color:var(--muted)">شاركنا فكرة مشروعك وسنرد عليك خلال 24 ساعة</p>
          <div class="meta">
            <span>خبرة +6 سنوات</span>
            <span>عميل سعيد</span>
            <span>دعم كامل</span>
          </div>
        </div>
      </div>
    </div>
  </header>

  <main class="container">
    <!-- Services -->
    <section id="services" class="section">
      <div class="card">
        <h2 style="color:var(--primary);margin-top:0">خدماتنا</h2>
        <div class="services" style="margin-top:12px">
          <div class="service">
            <h3>برمجة مواقع احترافية</h3>
            <p style="color:var(--muted);margin:6px 0 0">مواقع عرض، متاجر إلكترونية، بوابات للدفع، وواجهات مستخدم سريعة.</p>
          </div>
          <div class="service">
            <h3>برمجة تطبيقات موبايل</h3>
            <p style="color:var(--muted);margin:6px 0 0">تطبيقات أندرويد وiOS أصلية أو هجينـة مع أفضل ممارسات الأداء.</p>
          </div>
          <div class="service">
            <h3>حلول مخصصة وأنظمة</h3>
            <p style="color:var(--muted);margin:6px 0 0">أنظمة داخلية، إدارة موارد، واجهات API وربط بين الخدمات.</p>
          </div>
          <div class="service">
            <h3>صيانة ودعم</h3>
            <p style="color:var(--muted);margin:6px 0 0">خدمات صيانة، تحديثات أمنية، واستضافة مدارة.</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Features -->
    <section class="section">
      <div class="card">
        <h2 style="color:var(--primary);margin-top:0">لماذا تختار Big0Soft؟</h2>
        <div class="features" style="margin-top:12px">
          <div class="feature">
            <div class="dot">1</div>
            <div>
              <strong>حلول مخصصة</strong>
              <div style="color:var(--muted);margin-top:6px">نطوّر بما يلائم عملاءك وعملياتك، لا قوالب جاهزة.</div>
            </div>
          </div>

          <div class="feature">
            <div class="dot">✓</div>
            <div>
              <strong>تسليم ضمن المواعيد</strong>
              <div style="color:var(--muted);margin-top:6px">خارطة طريق واضحة وتسليم مرحلي مع تحديثات دورية.</div>
            </div>
          </div>

          <div class="feature">
            <div class="dot">⚙</div>
            <div>
              <strong>دعم فني مستمر</strong>
              <div style="color:var(--muted);margin-top:6px">حزمة صيانة ودعم بعد الإطلاق لضمان استقرار الخدمة.</div>
            </div>
          </div>

          <div class="feature">
            <div class="dot">🔒</div>
            <div>
              <strong>أمان وخصوصية</strong>
              <div style="color:var(--muted);margin-top:6px">تطبيق أفضل معايير الحماية وحماية بيانات المستخدمين.</div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Works -->
    <section id="works" class="section">
      <div class="card">
        <h2 style="color:var(--primary);margin-top:0">أعمالنا</h2>
        <div class="works" style="margin-top:12px">
          <div class="work">مشروع التجارة الإلكترونية</div>
          <div class="work">تطبيق حجز مواعيد</div>
          <div class="work">نظام إدارة موارد</div>
          <div class="work">بوابة دفع إلكتروني</div>
        </div>
      </div>
    </section>

    <!-- Testimonials & Contact -->
    <section class="section">
      <div style="display:grid;grid-template-columns:1fr 360px;gap:20px">
        <div class="card">
          <h2 style="color:var(--primary);margin-top:0">آراء العملاء</h2>
          <div class="testimonials" style="margin-top:12px">
            <div class="test">"تعامل احترافي وتسليم سريع" — عميل A</div>
            <div class="test">"كفاءة عالية وجودة في التنفيذ" — عميل B</div>
          </div>
        </div>

        <aside class="card">
          <h3 style="margin-top:0;color:var(--primary)">تواصل سريع</h3>
          <p style="color:var(--muted);margin-top:6px">اختر طريقة التواصل المفضلة لديك</p>
          <div style="display:flex;gap:8px;margin-top:12px;flex-direction:column">
            <a class="btn btn-whatsapp" href="https://wa.me/0000000000?text=مرحبًا%20Big0Soft!%20أرغب%20بخدمة%20" target="_blank" rel="noopener">📱 واتساب</a>
            <a class="btn btn-mail" href="https://mail.google.com/mail/?view=cm&fs=1&to=contact@big0soft.com" target="_blank" rel="noopener">✉️ جيميل</a>
          </div>
        </aside>
      </div>
    </section>

    <!-- Full Contact Form -->
    <section id="contact" class="section">
      <div class="card">
        <h2 style="color:var(--primary);margin-top:0">تواصل معنا</h2>
        <div class="contact-grid" style="margin-top:12px">
          <div>
            <form id="contactForm" onsubmit="return handleForm(event)">
              <input type="text" id="name" placeholder="الاسم" required>
              <input type="email" id="email" placeholder="البريد الإلكتروني" required>
              <input type="text" id="company" placeholder="اسم الشركة (اختياري)">
              <textarea id="message" rows="6" placeholder="اكتب رسالتك أو فكرة المشروع" required></textarea>
              <button type="submit">ارسل الرسالة</button>
              <p id="formMsg" style="margin-top:8px;color:var(--muted);font-size:13px"></p>
            </form>
          </div>

          <div>
            <div class="card" style="padding:14px">
              <h4 style="margin:0 0 8px">معلومات الاتصال</h4>
              <p style="margin:0;color:var(--muted)">📧 contact@big0soft.com</p>
              <p style="margin:6px 0 0;color:var(--muted)">📱 واتساب: +0000000000 (قم بتعديل الرقم)</p>
              <div style="height:12px"></div>
              <h4 style="margin:0 0 8px">ساعات العمل</h4>
              <p style="margin:0;color:var(--muted)">السبت - الخميس: 9:00 - 18:00</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container">
      <div class="footer-inner">
        <div class="small">&copy; 2025 Big0Soft — جميع الحقوق محفوظة</div>
        <div style="color:var(--muted);font-size:13px">صمم بواسطة Big0Soft</div>
      </div>
    </div>
  </footer>

  <!-- Floating WhatsApp button -->
  <a class="whatsapp-fab" href="https://wa.me/0000000000?text=مرحبًا%20Big0Soft!%20أرغب%20بخدمة%20" target="_blank" rel="noopener">📲 واتساب</a>

  <script>
    // بسيط: تبديل اللغة (عربي <-> إنجليزي)
    function toEnglish(){
      document.documentElement.lang='en';document.documentElement.dir='ltr';
      // نصوص إنجليزية
      document.querySelector('header .brand h1').textContent='Big0Soft';
      document.querySelector('header .brand div div').textContent='Professional software solutions — Web & Mobile';
      document.querySelectorAll('nav a')[0].textContent='Services';
      document.querySelectorAll('nav a')[1].textContent='Work';
      document.querySelectorAll('nav a')[2].textContent='Contact';
      document.querySelector('.hero .copy h2').textContent='Build stronger digital experiences for your business';
      document.querySelector('.hero .copy p').textContent='We design and develop professional websites and mobile apps that help your business grow.';
      document.querySelector('.btn-whatsapp').textContent='📱 Contact on WhatsApp';
      document.querySelector('.btn-mail').textContent='✉️ Email us (Gmail)';
      document.querySelector('#services h2').textContent='Services';
      document.querySelector('#works h2').textContent='Our Work';
      document.querySelector('#contact h2').textContent='Contact Us';
      document.querySelector('footer .small').textContent='© 2025 Big0Soft — All rights reserved';
    }

    function toArabic(){
      document.documentElement.lang='ar';document.documentElement.dir='rtl';
      // إعادة النصوص العربية الافتراضية
      location.reload(); // reload to quickly restore original Arabic text
    }

    // Form handling: مجرد محاكاة إرسال (يمكن ربط بالـ backend لاحقًا)
    function handleForm(e){
      e.preventDefault();
      const name=document.getElementById('name').value.trim();
      const email=document.getElementById('email').value.trim();
      const message=document.getElementById('message').value.trim();
      const formMsg=document.getElementById('formMsg');
      if(!name||!email||!message){formMsg.textContent='الرجاء ملء الحقول المطلوبة.';return}
      // هنا يمكنك استبدالها بطلب fetch إلى API سيرفرك
      formMsg.style.color='green';formMsg.textContent='تم إرسال رسالتك! سنعاود الاتصال بك قريبًا.';
      // reset form
      document.getElementById('contactForm').reset();
      return false;
    }

    // keyboard shortcut L to toggle language (لأغراض التجربة)
    document.addEventListener('keydown',function(e){
      if(e.key.toLowerCase()==='l'){
        if(document.documentElement.lang==='ar') toEnglish(); else toArabic();
      }
    });
  </script>
</body>
</html>
