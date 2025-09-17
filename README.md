<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>منصة سند | خدمات طلابية متكاملة — جامعة الملك سعود وما بعدها</title>
  <meta name="description" content="منصة سند: حلول واجبات وكويزات، مشاريع وتقارير، عروض تقديمية، ملخصات ومراجعات. نخدم جميع المواد والتخصصات بجامعة الملك سعود وغيرها. دعم سريع وموثوق." />
  <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet" />
  <style>
    :root{
      /* لوحة ألوان مستوحاة من KSU */
      --ksu-blue:#0B5BA9;      /* أزرق رئيسي */
      --ksu-deep:#0A3E78;      /* أزرق داكن */
      --ksu-sky:#2BA6FF;       /* أزرق فاتح */
      --ksu-mint:#13C3C1;      /* لمسة تركواز */
      --ink:#0f172a; --muted:#64748b;
      --bg:#f3f7fc; --card:#ffffff; --ring:#e2e8f0;
      --rad:16px;
      --shadow:0 10px 30px rgba(11,91,169,.12);
    }
    *{box-sizing:border-box}
    html,body{margin:0;scroll-behavior:smooth}
    body{font-family:'Tajawal',system-ui,sans-serif;color:var(--ink);background:
      radial-gradient(1200px 600px at 110% -10%, #eaf4ff 10%, transparent 60%),
      radial-gradient(900px 500px at -10% 110%, #e6fbff 10%, transparent 60%),
      var(--bg);
      line-height:1.85}
    a{color:var(--ksu-blue);text-decoration:none}
    .wrap{max-width:1200px;margin:auto;padding:28px 18px}

    /* HERO */
    .hero{
      background:
        linear-gradient(135deg, var(--ksu-deep) 0%, var(--ksu-blue) 65%, var(--ksu-sky) 100%);
      color:#fff; padding:64px 18px 48px; text-align:center; position:relative; overflow:hidden;
    }
    .hero::after{content:""; position:absolute; inset:auto -20% -40% -20%; height:260px;
      background:radial-gradient(500px 140px at 50% 0, rgba(255,255,255,.24), transparent 56%);
      filter:blur(10px);}
    .brand{display:inline-flex;gap:10px;align-items:center; padding:10px 16px; border-radius:999px;
      background:rgba(255,255,255,.15); border:1px solid rgba(255,255,255,.25); backdrop-filter: blur(6px);
      font-weight:800; letter-spacing:.3px}
    h1{margin:14px 0 6px; font-size:clamp(26px,4.5vw,38px)}
    p.lead{margin:0 auto 18px; color:#e9f2ff; max-width:800px}

    .cta-set{display:flex; gap:12px; flex-wrap:wrap; justify-content:center; margin-top:14px}
    .btn{display:inline-block; padding:12px 18px; border-radius:12px; font-weight:800;
      border:1px solid transparent; box-shadow:var(--shadow); transition:.2s}
    .btn.primary{background:#fff; color:var(--ksu-deep)}
    .btn.secondary{background:transparent; color:#fff; border-color:#ffffff66}
    .btn:hover{transform:translateY(-2px)}
    nav.top{display:flex; gap:14px; flex-wrap:wrap; justify-content:center; margin-top:18px}
    nav.top a{color:#fff; font-weight:700; opacity:.95}
    .kpis{display:grid; grid-template-columns:repeat(3,minmax(0,1fr)); gap:14px; margin-top:18px}
    .kpi{background:rgba(255,255,255,.12); border:1px solid #ffffff36; color:#eaf3ff;
      border-radius:14px; padding:12px}

    /* Sections */
    .section{padding:42px 0}
    h2{font-size:clamp(22px,3.2vw,28px); margin:0 0 14px; color:var(--ksu-deep)}
    .grid{display:grid; gap:18px}
    .cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}
    .cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}
    .card{background:var(--card); border:1px solid var(--ring); border-radius:var(--rad);
      padding:18px; box-shadow:var(--shadow)}
    .card h3{margin:0 0 6px}
    .tag{display:inline-block; margin:6px 6px 0 0; padding:4px 10px; border-radius:999px;
      background:#E9F2FF; color:#0B5BA9; font-weight:700; font-size:13px}

    /* Form */
    .form{background:#fff; border:1px solid var(--ring); border-radius:var(--rad); padding:18px; box-shadow:var(--shadow)}
    .row{display:grid; grid-template-columns:1fr 1fr; gap:12px}
    label{font-weight:700; color:#1f2a44; font-size:14px}
    input,select,textarea{
      width:100%; padding:12px 12px; border:1px solid var(--ring); border-radius:12px;
      background:#f9fbff; font-family:inherit; font-size:15px; outline:none
    }
    textarea{min-height:120px; resize:vertical}
    .form .btn{box-shadow:none}
    .hint{color:var(--muted); font-size:13px}

    /* FAQ & Footer */
    details{border:1px solid var(--ring); border-radius:12px; background:#fff; padding:10px 14px}
    details+details{margin-top:10px}
    details summary{cursor:pointer; font-weight:800; color:var(--ksu-deep)}
    footer{background:var(--ksu-deep); color:#cfe6ff; text-align:center; padding:22px}
    footer a{color:#93d5ff}

    /* Modal */
    .backdrop{position:fixed; inset:0; display:none; align-items:center; justify-content:center;
      background:rgba(3, 17, 43, .55); z-index:60; padding:16px}
    .modal{background:#fff; border:1px solid var(--ring); border-radius:18px; max-width:620px; width:100%;
      padding:18px}
    .copy{display:flex; gap:10px; align-items:center; margin:6px 0}
    .copy input{background:#f7fbff; border-radius:10px; border:1px solid var(--ring); padding:9px 10px; font-family:monospace}
    .sm{font-size:13px; color:var(--muted)}
    .ghost{background:transparent; color:var(--ksu-deep); border:1px solid var(--ring)}
    @media (max-width:900px){ .cols-3{grid-template-columns:1fr 1fr} }
    @media (max-width:640px){
      .cols-3,.cols-2{grid-template-columns:1fr}
      .row{grid-template-columns:1fr}
      .cta-set .btn{width:100%}
    }
  </style>
</head>
<body>

<!-- HERO -->
<header class="hero">
  <div class="wrap">
    <span class="brand">منصة سند — خدمات طلابية</span>
    <h1>خدمات متكاملة لكل المواد والتخصصات</h1>
    <p class="lead">حل واجبات وكويزات • مشاريع وتقارير • عروض تقديمية • ملخصات ومراجعات — بدعم سريع وموثوق.</p>
    <div class="cta-set">
      <a class="btn primary" href="#order">اطلب خدمتك الآن</a>
      <a class="btn secondary" href="#services">تعرّف على خدماتنا</a>
      <a class="btn secondary" href="https://t.me/iTx7llxb_15">تواصل تيليجرام</a>
      <a class="btn secondary" href="#" onclick="openPay()">بيانات التحويل اليدوي</a>
    </div>
    <nav class="top">
      <a href="#services">الخدمات</a>
      <a href="#disciplines">التخصصات</a>
      <a href="#packages">الباقات</a>
      <a href="#store">المتجر</a>
      <a href="#faq">الأسئلة</a>
      <a href="#order">طلب خدمة</a>
    </nav>
    <div class="kpis">
      <div class="kpi">⏱️ استجابة فورية عبر الخاص</div>
      <div class="kpi">🗓️ تسليم ضمن الوقت المتفق</div>
      <div class="kpi">🛡️ أعمال خاصة لضمان القبول</div>
    </div>
  </div>
</header>

<!-- الخدمات -->
<section id="services" class="section">
  <div class="wrap">
    <h2>ماذا نقدّم؟</h2>
    <div class="grid cols-3">
      <div class="card">
        <h3>📝 حل واجبات وكويزات</h3>
        <p>حلول دقيقة مع شرح مختصر عند الطلب + متابعة حتى الاعتماد.</p>
        <span class="tag">LMS/BB</span><span class="tag">تايمر</span><span class="tag">فل مارك</span>
      </div>
      <div class="card">
        <h3>📊 مشاريع وبحوث وتقارير</h3>
        <p>تحضير وكتابة وتنسيق ومراجع موثوقة حسب دليل المقرر.</p>
        <span class="tag">APA/IEEE</span><span class="tag">Case Study</span>
      </div>
      <div class="card">
        <h3>🎥 عروض تقديمية</h3>
        <p>بوربوينت حديث بخطوط واضحة وأيقونات ورسوم مبسّطة.</p>
        <span class="tag">عربي/إنجليزي</span>
      </div>
      <div class="card">
        <h3>📚 ملخصات ومراجعات</h3>
        <p>مفهرسة للميد والفاينل + تجميعات مختارة وخرائط ذهنية.</p>
        <span class="tag">مواد مشتركة</span><span class="tag">تحضيري</span>
      </div>
      <div class="card">
        <h3>📡 قنوات خاصة</h3>
        <p>متابعة مخصّصة للمشتركين عبر قنوات تيليجرام.</p>
        <span class="tag">تنبيهات مهام</span>
      </div>
      <div class="card">
        <h3>🎯 استشارات سريعة</h3>
        <p>اختيار موضوع، خطة مشروع، أو ترتيب الخطة الدراسية.</p>
        <span class="tag">15–30 دقيقة</span>
      </div>
    </div>
  </div>
</section>

<!-- التخصصات -->
<section id="disciplines" class="section" style="background:#fff">
  <div class="wrap">
    <h2>نغطي جميع المواد والتخصصات</h2>
    <div class="grid cols-3">
      <div class="card"><h3>📌 التحضيري والمشتركة</h3><ul><li>نهج 101، فجب/فكال 101، تقن 101، عرب 100، ENGL</li><li>مهارات جامعية، ريادة أعمال، ثقافة صحية</li></ul></div>
      <div class="card"><h3>🧪 العلوم</h3><ul><li>فيزياء/كيمياء/أحياء عامة ومخبرية</li><li>رياضيات وإحصاء</li></ul></div>
      <div class="card"><h3>💻 الحاسب</h3><ul><li>Python/Java/C/C#</li><li>هياكل بيانات، قواعد بيانات، شبكات</li></ul></div>
      <div class="card"><h3>🛠️ الهندسة</h3><ul><li>ميكانيكا، كهرباء، مدني، صناعي</li><li>تقارير مخبرية وتصاميم</li></ul></div>
      <div class="card"><h3>📈 الإدارة والأعمال</h3><ul><li>محاسبة، تمويل، تسويق</li><li>دراسات حالة وعروض</li></ul></div>
      <div class="card"><h3>🏥 التمريض والصحية</h3><ul><li>Case Study، تقارير تدريب</li><li>بحوث لياقة وتعليم صحي</li></ul></div>
      <div class="card"><h3>🎓 إنسانيات ولغات</h3><ul><li>تحليل نصوص، عروض أدبية</li><li>ترجمة وكتابة أكاديمية</li></ul></div>
      <div class="card"><h3>⚖️ القانون والتربية</h3><ul><li>بحوث قانونية</li><li>منهجيات تربوية</li></ul></div>
      <div class="card"><h3>… وغيرها</h3><p>ارسل اسم المادة والتفاصيل ونضبط لك الخطة بسرعة.</p></div>
    </div>
  </div>
</section>

<!-- الباقات -->
<section id="packages" class="section">
  <div class="wrap">
    <h2>الباقات (إرشادية)</h2>
    <div class="grid cols-3">
      <div class="card">
        <h3>أساسي</h3>
        <p><b>ابتداءً من 150 ر.س</b></p>
        <ul><li>حل واجبات فردية</li><li>ملخصات مختصرة</li><li>تسليم سريع</li></ul>
        <a class="btn primary" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20أساسي">اطلب الآن</a>
      </div>
      <div class="card" style="border:2px solid var(--ksu-blue)">
        <h3>الأكثر طلبًا — قياسي</h3>
        <p><b>ابتداءً من 200 ر.س</b></p>
        <ul><li>حل واجبات + كويزات</li><li>ملخصات مفهرسة</li><li>متابعة عبر الخاص</li></ul>
        <a class="btn primary" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20قياسي">اطلب الآن</a>
      </div>
      <div class="card">
        <h3>بريميوم</h3>
        <p><b>ابتداءً من 250 ر.س</b></p>
        <ul><li>حل شامل + مشاريع/تقارير</li><li>قنوات خاصة + مراجعات</li><li>دعم أولوية</li></ul>
        <a class="btn primary" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20بريميوم">اطلب الآن</a>
      </div>
    </div>
  </div>
</section>

<!-- المتجر -->
<section id="store" class="section" style="background:#fff">
  <div class="wrap">
    <h2>🛍️ متجر الملخصات والملازم</h2>
    <p>ملخصات وتجميعات للميد والفاينل — مرتبة وجاهزة للمذاكرة.</p>
    <div class="cta-set">
      <a class="btn primary" href="https://t.me/Helping_KSU">فتح المتجر في تيليجرام</a>
      <a class="btn secondary" href="https://t.me/iTx7llxb_15">طلبات خاصة</a>
    </div>
  </div>
</section>

<!-- طلب خدمة -->
<section id="order" class="section">
  <div class="wrap">
    <h2>نموذج طلب الخدمة</h2>
    <p class="hint">املأ الحقول التالية وسيتم توليد رسالة جاهزة للإرسال على واتساب أو تيليجرام.</p>
    <form class="form" onsubmit="return false;">
      <div class="row">
        <div>
          <label>الاسم</label>
          <input id="name" placeholder="اسمك الثلاثي" />
        </div>
        <div>
          <label>الجامعة/الكلية</label>
          <input id="uni" placeholder="مثال: KSU — كلية العلوم" />
        </div>
      </div>
      <div class="row">
        <div>
          <label>اسم المقرر</label>
          <input id="course" placeholder="مثال: STAT 1100 / نهج 101" />
        </div>
        <div>
          <label>نوع الخدمة</label>
          <select id="type">
            <option value="حل واجب">حل واجب</option>
            <option value="كويز تايمر">كويز تايمر</option>
            <option value="مشروع/تقرير">مشروع/تقرير</option>
            <option value="عرض تقديمي">عرض تقديمي</option>
            <option value="ملخص/مراجعة">ملخص/مراجعة</option>
            <option value="أخرى">أخرى</option>
          </select>
        </div>
      </div>
      <div class="row">
        <div>
          <label>الموعد النهائي</label>
          <input id="due" type="datetime-local" />
          <div class="hint">اكتب الوقت والتاريخ بدقة.</div>
        </div>
        <div>
          <label>الدرجة/المتطلبات</label>
          <input id="grade" placeholder="مثال: فل مارك / قبول فقط / شروط دكتور" />
        </div>
      </div>
      <div>
        <label>تفاصيل إضافية</label>
        <textarea id="details" placeholder="رابط المهمة/الوصف المختصر + أي ملاحظات مهمة (الملفات/عدد الصفحات/أسلوب التوثيق...)"></textarea>
      </div>
      <div class="row">
        <div>
          <label>طريقة التواصل المفضلة</label>
          <select id="channel">
            <option value="whatsapp">واتساب</option>
            <option value="telegram">تيليجرام</option>
          </select>
        </div>
        <div>
          <label>وسيلة الدفع</label>
          <select id="pay">
            <option value="نجوم تيليجرام/بطاقات">نجوم تيليجرام/بطاقات</option>
            <option value="تحويل بنكي/‏STC Pay">تحويل بنكي/‏STC Pay</option>
            <option value="تنسيق لاحق">تنسيق لاحق</option>
          </select>
        </div>
      </div>

      <div class="cta-set" style="margin-top:14px">
        <button class="btn primary" onclick="sendWhatsApp()">إرسال واتساب</button>
        <button class="btn ghost" onclick="sendTelegram()">إرسال تيليجرام</button>
        <button class="btn secondary" type="reset">مسح النموذج</button>
      </div>

      <p class="hint">بالضغط على الإرسال سيتم فتح تطبيق المراسلة برسالة مُنسّقة تلقائيًا، ويمكنك تعديلها قبل الإرسال.</p>
    </form>
  </div>
</section>

<!-- الأسئلة -->
<section id="faq" class="section" style="background:#fff">
  <div class="wrap">
    <h2>الأسئلة الشائعة</h2>
    <details><summary>كيف يتم التسليم؟</summary><p>على واتساب/تيليجرام أو عبر قناة المادة الخاصة حسب الخدمة.</p></details>
    <details><summary>هل تتوفر أقساط؟</summary><p>نعم لبعض المشاريع والباقات؛ يتم الاتفاق قبل البدء.</p></details>
    <details><summary>هل العمل خاص وغير مكرر؟</summary><p>نعم، كل عمل مُخصّص لضمان القبول وعدم التكرار وبتوثيق مناسب.</p></details>
  </div>
</section>

<!-- بيانات التحويل اليدوي -->
<div id="payModal" class="backdrop" role="dialog" aria-modal="true" aria-hidden="true">
  <div class="modal">
    <h3>🏦 بيانات التحويل اليدوي (STC Pay / بنك محلي)</h3>
    <p class="sm">بعد التحويل أرسل الإيصال ليتم تأكيد الطلب بسرعة — توصلك رسالة تلقائيًا.</p>
    <div class="card" style="margin:10px 0">
      <div class="copy"><b>البنك:</b> البنك العربي الوطني السعودي (anb)</div>
      <div class="copy"><span>👤 اسم المستفيد:</span><input id="benef" value="عزام عبدالله عبدالعزيز ناجي" readonly /><button class="btn ghost" onclick="cp('benef')">نسخ</button></div>
      <div class="copy"><span># رقم الحساب:</span><input id="acc" value="942000177167245" readonly /><button class="btn ghost" onclick="cp('acc')">نسخ</button></div>
      <div class="copy"><span>💳 الآيبان:</span><input id="iban" value="SA0530100942000177167245" readonly /><button class="btn ghost" onclick="cp('iban')">نسخ</button></div>
      <ul class="sm">
        <li>لو بنكك مختلف (راجحي/أهلي/…): الصق الآيبان واسم المستفيد وحوّل عادي.</li>
      </ul>
    </div>
    <div class="cta-set">
      <a class="btn primary" href="https://wa.me/966565885750?text=تم%20التحويل%20وهذا%20الإيصال">إرفاق الإيصال عبر واتساب</a>
      <button class="btn ghost" onclick="closePay()">إغلاق</button>
    </div>
  </div>
</div>

<footer>
  <div class="wrap">
    <p>© <span id="y"></span> منصة سند للخدمات الإلكترونية والتعليمية — جميع الحقوق محفوظة.</p>
    <p><a href="https://t.me/Helping_KSU">قناة المتجر</a> • <a href="https://t.me/student_services24">قناة الأعمال</a> • <a href="#order">اطلب خدمة</a></p>
  </div>
</footer>

<script>
  // سنة الحقوق
  document.getElementById('y').textContent = new Date().getFullYear();

  // فتح/إغلاق مودال الدفع
  function openPay(){const b=document.getElementById('payModal'); b.style.display='flex'; b.setAttribute('aria-hidden','false')}
  function closePay(){const b=document.getElementById('payModal'); b.style.display='none'; b.setAttribute('aria-hidden','true')}
  document.getElementById('payModal').addEventListener('click',e=>{ if(e.target.id==='payModal') closePay(); });

  // نسخ
  function cp(id){ const el=document.getElementById(id); el.select(); el.setSelectionRange(0,99999); document.execCommand('copy'); alert('تم النسخ ✅'); }

  // بناء الرسالة الموحدة
  function buildMessage(){
    const name = (document.getElementById('name').value||'').trim();
    const uni  = (document.getElementById('uni').value||'').trim();
    const course = (document.getElementById('course').value||'').trim();
    const type = document.getElementById('type').value;
    const due  = document.getElementById('due').value;
    const grade= (document.getElementById('grade').value||'').trim();
    const details=(document.getElementById('details').value||'').trim();
    const pay = document.getElementById('pay').value;

    // قالب منسق
    const msg = `*طلب خدمة — منصة سند*%0A%0A` +
      `الاسم: ${name||'-'}%0A` +
      `الجامعة/الكلية: ${uni||'-'}%0A` +
      `المقرر: ${course||'-'}%0A` +
      `نوع الخدمة: ${type}%0A` +
      `الموعد النهائي: ${due||'-'}%0A` +
      `الدرجة/المتطلبات: ${grade||'-'}%0A` +
      `وسيلة الدفع: ${pay}%0A%0A` +
      `تفاصيل إضافية:%0A${encodeURIComponent(details||'-')}%0A%0A` +
      `🔎 من فضلك أكد الاستلام وحدد السعر المناسب لكم.`;

    return msg;
  }

  function sendWhatsApp(){
    const msg = buildMessage();
    const url = `https://wa.me/966565885750?text=${msg}`;
    window.open(url, '_blank');
  }
  function sendTelegram(){
    const msg = buildMessage();
    const url = `https://t.me/iTx7llxb_15?text=${msg}`;
    window.open(url, '_blank');
  }
</script>

</body>
</html>
