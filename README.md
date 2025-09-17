<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>منصة سند للخدمات الإلكترونية والتعليمية | خدمات طلابية لجميع المواد والتخصصات</title>
  <meta name="description" content="منصة سند: حلول واجبات وكويزات، مشاريع وتقارير، عروض تقديمية، ملخصات ومراجعات. نخدم جميع المواد والتخصصات بجامعة الملك سعود وغيرها. دعم سريع وموثوق." />
  <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;600;700&display=swap" rel="stylesheet" />
  <style>
    :root{
      --ink:#0f172a; --ink-2:#1e293b; --brand:#2563eb; --sky:#38bdf8; --bg:#f8fafc; --card:#ffffff; --muted:#64748b; --ring:#e2e8f0;
      --radius:14px;
    }
    *{box-sizing:border-box}
    body{margin:0;background:var(--bg);color:var(--ink);font-family:'Tajawal',sans-serif;line-height:1.8}
    a{color:var(--brand);text-decoration:none}
    header.hero{background:linear-gradient(135deg,#0f172a 0%,#1e293b 60%);color:#fff;padding:48px 16px;text-align:center}
    .wrap{max-width:1100px;margin:auto;padding:24px 16px}
    nav.top{display:flex;gap:14px;flex-wrap:wrap;justify-content:center;margin-top:10px}
    nav.top a{color:#fff;font-weight:700}
    .pill{display:inline-block;padding:10px 14px;border-radius:999px;background:#fff;color:var(--ink);font-weight:700}
    .btn{display:inline-block;padding:11px 16px;border-radius:10px;background:var(--ink);color:#fff;font-weight:700;border:1px solid transparent}
    .btn:hover{background:#1d4ed8}
    .btn.ghost{background:#0000;color:#fff;border-color:#fff}
    .section{padding:36px 0}
    h1,h2,h3{margin:0 0 10px}
    h2{font-size:26px}
    p.lead{color:#e2e8f0}
    .grid{display:grid;gap:18px}
    .grid.cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}
    .grid.cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}
    .card{background:var(--card);border:1px solid var(--ring);border-radius:var(--radius);padding:18px;box-shadow:0 3px 10px rgba(2,8,23,.06)}
    .card h3{margin:0 0 6px}
    .tag{display:inline-block;margin:0 6px 6px 0;padding:4px 10px;border-radius:999px;background:#eef2ff;color:#1e3a8a;font-weight:600;font-size:13px}
    details{border:1px solid var(--ring);border-radius:10px;background:#fff;padding:10px 14px}
    details+details{margin-top:10px}
    details summary{cursor:pointer;font-weight:700;color:var(--ink-2)}
    ul{margin:8px 0 0 0;padding:0 0 0 18px}
    .kpis{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:14px;margin-top:14px}
    .kpi{background:#0ea5e90d;border:1px solid var(--ring);border-radius:12px;padding:12px;text-align:center}
    .kpi b{display:block;font-size:20px}
    .cta-set{display:flex;gap:10px;flex-wrap:wrap;margin-top:14px}
    footer{background:var(--ink);color:#94a3b8;padding:18px;text-align:center;margin-top:40px}
    footer a{color:var(--sky)}
    /* Responsive */
    @media (max-width:900px){ .grid.cols-3{grid-template-columns:1fr 1fr} }
    @media (max-width:640px){
      .grid.cols-3,.grid.cols-2{grid-template-columns:1fr}
      nav.top{flex-direction:column}
      .btn, .pill{width:100%;text-align:center}
    }
    /* modal */
    .modal-backdrop{position:fixed;inset:0;background:rgba(15,23,42,.6);display:none;align-items:center;justify-content:center;padding:16px;z-index:50}
    .modal{background:#fff;border-radius:16px;max-width:560px;width:100%;padding:18px;border:1px solid var(--ring)}
    .modal h3{margin:0 0 10px}
    .row{display:flex;gap:10px;align-items:center}
    .copy{padding:8px 10px;border-radius:8px;border:1px solid var(--ring);background:#f8fafc;font-family:monospace}
    .icon{font-weight:900}
  </style>
</head>
<body>

<!-- HERO -->
<header class="hero">
  <div class="wrap">
    <span class="pill">منصة سند للخدمات الإلكترونية والتعليمية</span>
    <h1 style="margin-top:10px">خدمات طلابية متكاملة — لكل المواد والتخصصات</h1>
    <p class="lead">حل واجبات وكويزات • مشاريع وتقارير • عروض تقديمية • ملخصات ومراجعات — دعم سريع وموثوق</p>

    <div class="cta-set">
      <a class="btn" href="#services">تعرّف على خدماتنا</a>
      <a class="btn ghost" href="https://t.me/iTx7llxb_15">تواصل عبر تيليجرام</a>
      <a class="btn ghost" href="#" onclick="openPay()">بيانات التحويل اليدوي</a>
    </div>

    <nav class="top" style="margin-top:18px">
      <a href="#services">الخدمات</a>
      <a href="#disciplines">التخصصات</a>
      <a href="#packages">الباقات</a>
      <a href="#store">المتجر</a>
      <a href="#faq">الأسئلة</a>
      <a href="#contact">تواصل</a>
    </nav>

    <div class="kpis">
      <div class="kpi"><b>⏱️ استجابة سريعة</b>متابعة فورية عبر الخاص</div>
      <div class="kpi"><b>📦 تسليم ضمن الوقت</b>خطة واضحة ومواعيد دقيقة</div>
      <div class="kpi"><b>🛡️ عمل خاص</b>بدون تكرار لضمان القبول</div>
    </div>
  </div>
</header>

<!-- الخدمات -->
<section id="services" class="section">
  <div class="wrap">
    <h2>ماذا نقدّم؟</h2>
    <p>باقة خدمات تعليمية مرنة تناسب احتياجك في التحضيري والمواد المشتركة وجميع الكليات.</p>

    <div class="grid cols-3">
      <div class="card">
        <h3>📝 حل واجبات وكويزات</h3>
        <p>حلول دقيقة مع شرح مختصر عند الطلب + متابعة حتى الاعتماد.</p>
        <span class="tag">واجبات LMS/BB</span><span class="tag">كويزات تايمر</span><span class="tag">فل مارك</span>
      </div>

      <div class="card">
        <h3>📊 مشاريع وبحوث وتقارير</h3>
        <p>تنفيذ كامل (تحضير، كتابة، تنسيق، مصادر) وفق متطلبات المقرر.</p>
        <span class="tag">تقارير مخبرية</span><span class="tag">أبحاث APA/IEEE</span><span class="tag">دراسة حالة</span>
      </div>

      <div class="card">
        <h3>🎥 عروض تقديمية</h3>
        <p>تصميم بوربوينت حديث بخطوط واضحة وأيقونات ورسوم بسيطة.</p>
        <span class="tag">قوالب احترافية</span><span class="tag">لغة عربية/إنجليزية</span>
      </div>

      <div class="card">
        <h3>📚 ملخصات ومراجعات</h3>
        <p>ملخصات مفهرسة للميد والفاينل + تجميعات مهمّة مع خرائط ذهنية.</p>
        <span class="tag">مواد مشتركة</span><span class="tag">تحضيري</span><span class="tag">تخصص</span>
      </div>

      <div class="card">
        <h3>📡 قنوات خاصة</h3>
        <p>متابعة مخصّصة للمشتركين عبر قنوات تيليجرام بحسب المادة.</p>
        <span class="tag">تنبيهات مهام</span><span class="tag">روابط ومراجع</span>
      </div>

      <div class="card">
        <h3>🎯 استشارات سريعة</h3>
        <p>إرشاد بخصوص اختيار الموضوع، خطة المشروع، أو ترتيب الخطة الدراسية.</p>
        <span class="tag">15–30 دقيقة</span><span class="tag">اقتراحات موثوقة</span>
      </div>
    </div>
  </div>
</section>

<!-- التخصصات والمواد -->
<section id="disciplines" class="section" style="background:#fff">
  <div class="wrap">
    <h2>التغطية الأكاديمية — جميع المواد والتخصصات</h2>
    <p class="muted">نخدم جامعة الملك سعود وغيرها. هذه أمثلة وليست حصرًا:</p>

    <div class="grid cols-3">
      <div class="card">
        <h3>📌 التحضيري والمواد المشتركة</h3>
        <ul>
          <li>نهج 101، فجب/فكال 101، تقن 101، عرب 100، ENGL</li>
          <li>مهارات جامعية، ريادة أعمال، ثقافة صحية</li>
        </ul>
      </div>

      <div class="card">
        <h3>🧪 كلية العلوم</h3>
        <ul>
          <li>فيزياء/كيمياء/أحياء عامة ومخبرية</li>
          <li>رياضيات وإحصاء (تمارين، كويزات، مشاريع)</li>
        </ul>
      </div>

      <div class="card">
        <h3>💻 الحاسب وتقنية المعلومات</h3>
        <ul>
          <li>برمجة (Python/Java/C/C#)</li>
          <li>هياكل بيانات، قواعد بيانات، شبكات</li>
          <li>تقارير مشاريع وتوثيق (UML، ERD)</li>
        </ul>
      </div>

      <div class="card">
        <h3>🛠️ الهندسة</h3>
        <ul>
          <li>ميكانيكا، كهرباء، مدني، صناعي</li>
          <li>تقارير مخبرية، عروض التصميم، حسابات</li>
        </ul>
      </div>

      <div class="card">
        <h3>📈 الإدارة والأعمال</h3>
        <ul>
          <li>محاسبة، تمويل، تسويق، إدارة عمليات</li>
          <li>دراسات حالة، عروض، أبحاث سوق</li>
        </ul>
      </div>

      <div class="card">
        <h3>🏥 التمريض والعلوم الصحية</h3>
        <ul>
          <li>Case Study، بحث لياقة، تقارير تدريب</li>
          <li>عروض تعليم صحي، ملخصات مراجعة</li>
        </ul>
      </div>

      <div class="card">
        <h3>🎓 اللغات والإنساني</h3>
        <ul>
          <li>عروض أدبية، نقد، لغويات</li>
          <li>ترجمة، كتابة أكاديمية</li>
        </ul>
      </div>

      <div class="card">
        <h3>⚖️ القانون والتربية</h3>
        <ul>
          <li>بحوث قانونية ومنهجيات تربوية</li>
          <li>عروض سياسات وتعليم</li>
        </ul>
      </div>

      <div class="card">
        <h3>… وغيرها</h3>
        <p>أرسل اسم المادة والتفاصيل، ونضبط لك خطة مناسبة بسرعة.</p>
      </div>
    </div>
  </div>
</section>

<!-- الباقات -->
<section id="packages" class="section">
  <div class="wrap">
    <h2>الباقات والأسعار (إرشادية)</h2>
    <p>الأسعار تتغيّر حسب المادة والمحتوى والوقت — نحدّد لك السعر النهائي قبل البدء.</p>

    <div class="grid cols-3">
      <div class="card">
        <h3>أساسي</h3>
        <p><b>ابتداءً من 150 ر.س</b></p>
        <ul>
          <li>حل واجبات فردية</li>
          <li>ملخصات مختصرة</li>
          <li>تسليم سريع</li>
        </ul>
        <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20أساسي">اطلب الآن</a>
      </div>

      <div class="card" style="border:2px solid #2563eb">
        <h3>الأكثر طلبًا — قياسي</h3>
        <p><b>ابتداءً من 200 ر.س</b></p>
        <ul>
          <li>حل واجبات + كويزات</li>
          <li>ملخصات مفهرسة</li>
          <li>متابعة عبر الخاص</li>
        </ul>
        <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20قياسي">اطلب الآن</a>
      </div>

      <div class="card">
        <h3>بريميوم</h3>
        <p><b>ابتداءً من 250 ر.س</b></p>
        <ul>
          <li>حل شامل + مشاريع/تقارير</li>
          <li>قنوات خاصة + مراجعات</li>
          <li>دعم أولوية</li>
        </ul>
        <a class="btn" href="https://wa.me/966565885750?text=أرغب%20في%20باقة%20بريميوم">اطلب الآن</a>
      </div>
    </div>
  </div>
</section>

<!-- المتجر -->
<section id="store" class="section" style="background:#fff">
  <div class="wrap">
    <h2>🛍️ متجر الملخصات والملازم</h2>
    <p>مذكرات وملخصات وتجميعات للميد والفاينل — مرتبة وجاهزة للمذاكرة.</p>
    <div class="cta-set">
      <a class="btn" href="https://t.me/Helping_KSU">فتح المتجر في تيليجرام</a>
      <a class="btn ghost" href="https://t.me/iTx7llxb_15">طلبات خاصّة</a>
    </div>
  </div>
</section>

<!-- كيف نشتغل -->
<section class="section">
  <div class="wrap">
    <h2>كيف نشتغل؟</h2>
    <div class="grid cols-3">
      <div class="card"><h3>1) تواصل سريع</h3><p>ارسل تفاصيل المادة/المهمة على واتساب أو تيليجرام.</p></div>
      <div class="card"><h3>2) عرض وسعر</h3><p>نقدّم لك الخطة والسعر المناسب حسب الوقت والمحتوى.</p></div>
      <div class="card"><h3>3) تنفيذ وتسليم</h3><p>ننفّذ ونسلّم بالشكل المطلوب + متابعة حتى الاعتماد.</p></div>
    </div>
  </div>
</section>

<!-- الضمان -->
<section class="section" style="background:#fff">
  <div class="wrap">
    <h2>معاييرنا</h2>
    <div class="grid cols-3">
      <div class="card"><h3>✅ ثقة</h3><p>تعامل واضح وسجل إنجازات قوي.</p></div>
      <div class="card"><h3>✅ دقة</h3><p>تسليم منسّق ومراجع وخالٍ من الأخطاء.</p></div>
      <div class="card"><h3>✅ التزام</h3><p>مواعيد دقيقة ودعم بعد التسليم.</p></div>
    </div>
    <details style="margin-top:12px">
      <summary>تنبيه مهم</summary>
      <p>تجنّب النسخ/اللصق واستخدام الذكاء الاصطناعي بشكل غير منضبط؛ قد يرفع الاقتباس ويؤثر على الدرجات. نضمن أعمالًا خاصة لكل طالب.</p>
    </details>
  </div>
</section>

<!-- الأسئلة -->
<section id="faq" class="section">
  <div class="wrap">
    <h2>الأسئلة الشائعة</h2>
    <details><summary>كيف يتم التسليم؟</summary><p>على واتساب/تيليجرام أو عبر قناة المادة الخاصة حسب الخدمة.</p></details>
    <details><summary>هل تتوفر أقساط؟</summary><p>نعم لبعض المشاريع والباقات؛ يتم الاتفاق قبل البدء.</p></details>
    <details><summary>هل العمل خاص وغير مكرّر؟</summary><p>نعم، كل عمل مُخصّص لضمان القبول وعدم التكرار.</p></details>
  </div>
</section>

<!-- تواصل -->
<section id="contact" class="section" style="background:#fff">
  <div class="wrap">
    <h2>تواصل مباشر</h2>
    <div class="cta-set">
      <a class="btn" href="https://wa.me/966565885750">🟢 واتساب</a>
      <a class="btn" href="https://t.me/iTx7llxb_15">🔵 تيليجرام</a>
    </div>
    <p style="color:var(--muted);margin-top:8px">ساعات العمل: يوميًا 10 ص — 12 ص</p>
    <div class="cta-set">
      <a class="btn ghost" href="https://t.me/Helping_KSU">📣 قناة المتجر</a>
      <a class="btn ghost" href="https://t.me/student_services24">📢 قناة الأعمال</a>
    </div>
  </div>
</section>

<!-- Modal: بيانات التحويل -->
<div id="payModal" class="modal-backdrop" role="dialog" aria-modal="true" aria-hidden="true">
  <div class="modal">
    <h3>🏦 بيانات التحويل اليدوي (STC Pay / بنك محلي)</h3>
    <p style="margin:6px 0 12px">ادفع بأمان ثم أرسل الإيصال لتأكيد طلبك خلال وقت قصير؛ توصلك رسالة تلقائيًا.</p>

    <div class="card" style="margin-bottom:10px">
      <p><b>البنك:</b> البنك العربي الوطني السعودي (anb)</p>
      <div class="row" style="margin:8px 0">
        <span class="icon">👤</span><span style="min-width:110px">اسم المستفيد:</span>
        <input id="benef" class="copy" value="عزام عبدالله عبدالعزيز ناجي" readonly />
        <button class="btn" onclick="cp('benef')">نسخ</button>
      </div>
      <div class="row" style="margin:8px 0">
        <span class="icon">#</span><span style="min-width:110px">رقم الحساب:</span>
        <input id="acc" class="copy" value="942000177167245" readonly />
        <button class="btn" onclick="cp('acc')">نسخ</button>
      </div>
      <div class="row" style="margin:8px 0">
        <span class="icon">💳</span><span style="min-width:110px">الآيبان:</span>
        <input id="iban" class="copy" value="SA0530100942000177167245" readonly />
        <button class="btn" onclick="cp('iban')">نسخ</button>
      </div>
      <ul style="margin-top:8px">
        <li>بعد التحويل أرسل الإيصال على واتساب/البوت لتأكيد الطلب.</li>
        <li>لو بنكك مختلف (راجحي/أهلي/…): الصق الآيبان واسم المستفيد وحوّل عادي.</li>
      </ul>
    </div>

    <div class="cta-set">
      <a class="btn" href="https://wa.me/966565885750?text=تم%20التحويل%20وهذا%20الإيصال">إرفاق الإيصال عبر واتساب</a>
      <button class="btn ghost" onclick="closePay()">إغلاق</button>
    </div>
  </div>
</div>

<footer>
  <div class="wrap" style="text-align:center">
    <p>© منصة سند للخدمات الإلكترونية والتعليمية — جميع الحقوق محفوظة.</p>
    <p><a href="https://t.me/Helping_KSU">قناة المتجر</a> • <a href="https://t.me/student_services24">قناة الأعمال</a></p>
  </div>
</footer>

<script>
  function openPay(){document.getElementById('payModal').style.display='flex'; document.getElementById('payModal').setAttribute('aria-hidden','false')}
  function closePay(){document.getElementById('payModal').style.display='none'; document.getElementById('payModal').setAttribute('aria-hidden','true')}
  function cp(id){const el=document.getElementById(id); el.select(); el.setSelectionRange(0, 99999); document.execCommand('copy'); alert('تم النسخ ✅');}
  // اقفال بالضغط خارج المودال
  document.getElementById('payModal').addEventListener('click',e=>{
    if(e.target.id==='payModal') closePay();
  });
</script>

</body>
</html>
