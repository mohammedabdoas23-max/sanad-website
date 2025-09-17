<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>منصة سند للخدمات الإلكترونية والتعليمية</title>
  <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body { font-family: 'Tajawal', sans-serif; margin: 0; padding: 0; background:#f9f9f9; color:#222; }
    header { background:#0f172a; color:#fff; padding:20px; text-align:center; }
    nav { background:#1e293b; display:flex; flex-wrap:wrap; justify-content:center; gap:15px; padding:10px; }
    nav a { color:#fff; text-decoration:none; font-weight:bold; }
    nav a:hover { color:#38bdf8; }
    section { padding:30px 15px; max-width:1100px; margin:auto; }
    h1, h2, h3 { color:#0f172a; margin-bottom:10px; }
    p { line-height:1.8; }
    .btn { background:#0f172a; color:#fff; padding:10px 15px; border-radius:8px; text-decoration:none; display:inline-block; margin-top:10px; transition:0.3s; }
    .btn:hover { background:#2563eb; }
    .cards { display:grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap:20px; margin-top:20px; }
    .card { background:#fff; border:1px solid #ddd; border-radius:10px; padding:20px; box-shadow:0 2px 4px rgba(0,0,0,0.1); transition:0.3s; }
    .card:hover { transform:translateY(-5px); box-shadow:0 4px 8px rgba(0,0,0,0.15); }
    details { background:#fff; border-radius:8px; padding:10px 15px; margin:8px 0; border:1px solid #ddd; }
    details summary { cursor:pointer; font-weight:bold; color:#0f172a; }
    footer { background:#0f172a; color:#fff; text-align:center; padding:15px; margin-top:40px; }
    footer a { color:#38bdf8; text-decoration:none; margin:0 8px; }
    footer a:hover { text-decoration:underline; }
    
    /* ✅ تحسينات للجوال */
    @media (max-width: 600px) {
      nav { flex-direction:column; align-items:center; }
      .btn { width:100%; text-align:center; }
      .cards { grid-template-columns:1fr; }
    }
  </style>
</head>
<body>

<header>
  <h1>منصة سند للخدمات الإلكترونية والتعليمية</h1>
  <p>خدمات طلابية متكاملة — حلول، مشاريع، عروض، ملخصات</p>
</header>

<nav>
  <a href="#services">الخدمات</a>
  <a href="#packages">الباقات</a>
  <a href="#store">المتجر</a>
  <a href="#about">من نحن</a>
  <a href="#faq">الأسئلة</a>
  <a href="#contact">تواصل</a>
</nav>

<section id="services">
  <h2>خدماتنا</h2>
  <div class="cards">
    <div class="card"><h3>حلول سريعة</h3><p>كويزات وواجبات مع ضمان الدقة.</p></div>
    <div class="card"><h3>مشاريع وتقارير</h3><p>تنفيذ كامل وتسليم مرتب.</p></div>
    <div class="card"><h3>عروض تقديمية</h3><p>تصاميم احترافية وواضحة.</p></div>
    <div class="card"><h3>ملخصات ومراجعات</h3><p>مفهرسة ومحدثة قبل الاختبارات.</p></div>
  </div>
</section>

<section id="packages">
  <h2>الباقات والأسعار</h2>
  <div class="cards">
    <div class="card">
      <h3>أساسي</h3>
      <p>ابتداءً من 150 ر.س</p>
      <ul>
        <li>حل واجبات فردية</li>
        <li>ملخصات مختصرة</li>
      </ul>
      <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20أساسي">اطلب الآن</a>
    </div>
    <div class="card">
      <h3>قياسي</h3>
      <p>ابتداءً من 200 ر.س</p>
      <ul>
        <li>حل واجبات + كويزات</li>
        <li>ملخصات مفهرسة</li>
        <li>متابعة خاصة</li>
      </ul>
      <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20قياسي">اطلب الآن</a>
    </div>
    <div class="card">
      <h3>بريميوم</h3>
      <p>ابتداءً من 250 ر.س</p>
      <ul>
        <li>حل شامل + مشاريع</li>
        <li>قناة خاصة + مراجعات</li>
        <li>دعم أولوية</li>
      </ul>
      <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20بريميوم">اطلب الآن</a>
    </div>
  </div>
</section>

<section id="store">
  <h2>🛍️ متجر الملخصات والملازم</h2>
  <p>مذكرات وتجميعات جاهزة للمذاكرة.</p>
  <a class="btn" href="https://t.me/Helping_KSU">فتح المتجر</a>
</section>

<section id="about">
  <h2>من نحن</h2>
  <p>فريق سند — كادر متكامل لخدمات طلابية موثوقة لجامعة الملك سعود وغيرها.</p>
  <ul>
    <li>✅ ثقة</li>
    <li>✅ دقة</li>
    <li>✅ التزام</li>
  </ul>
</section>

<section id="faq">
  <h2>الأسئلة الشائعة</h2>
  <details><summary>كيف يتم التسليم؟</summary><p>عبر الواتساب أو تيليجرام.</p></details>
  <details><summary>هل تتوفر أقساط؟</summary><p>نعم لبعض المشاريع والباقات.</p></details>
  <details><summary>هل العمل خاص وغير مكرر؟</summary><p>نعم لكل طالب عمل خاص لضمان القبول.</p></details>
</section>

<section id="contact">
  <h2>تواصل معنا</h2>
  <a class="btn" href="https://wa.me/966565885750">واتساب مباشر</a>
  <a class="btn" href="https://t.me/iTx7llxb_15">تيليجرام مباشر</a>
</section>

<footer>
  <p>© منصة سند للخدمات الإلكترونية والتعليمية. جميع الحقوق محفوظة.</p>
  <p>
    <a href="https://t.me/Helping_KSU">📣 قناة المتجر</a> •
    <a href="https://t.me/student_services24">📢 قناة الأعمال</a>
  </p>
</footer>

</body>
</html>