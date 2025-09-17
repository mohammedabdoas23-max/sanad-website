<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>منصة سند | خدمات طلابية متكاملة — جامعة الملك سعود (KSU)</title>
  <meta name="description" content="منصة سند — خدمات طلابية متكاملة: حلول واجبات وكويزات، مشاريع، عروض، ملخصات ومتابعة فصليّة لطلاب جامعة الملك سعود."/>
  <meta name="author" content="منصة سند — Sanad Platform" />
  <style>
    :root{
      --ksu-dark:#002b5c;    /* KSU deep blue */
      --ksu-mid:#0a4fa1;     /* accent */
      --bg:#f5f8fb;
      --card:#ffffff;
      --muted:#57606a;
      --gold:#f59e0b;
      --success:#16a34a;
      --radius:12px;
      --glass:rgba(255,255,255,0.7);
    }
    *{box-sizing:border-box}
    body{margin:0;font-family: "Noto Kufi Arabic", "Segoe UI", Tahoma, Arial, sans-serif;background:linear-gradient(180deg,var(--bg),#ffffff);color:#0b1220;line-height:1.5}
    .wrap{max-width:1180px;margin:20px auto;padding:16px}
    /* header */
    header.top{display:flex;align-items:center;gap:14px;padding:12px;border-radius:14px;background:linear-gradient(90deg,var(--ksu-dark),var(--ksu-mid));color:#fff;box-shadow:0 6px 18px rgba(3,37,77,0.12)}
    .logo{display:flex;align-items:center;gap:10px}
    .logo-box{width:64px;height:64px;border-radius:12px;background:#fff;display:flex;align-items:center;justify-content:center}
    .brand{font-weight:900;font-size:20px}
    .tag{font-size:13px;color:rgba(255,255,255,0.9)}
    .nav-actions{margin-left:auto;display:flex;gap:8px}
    .btn{padding:10px 14px;border-radius:10px;border:0;cursor:pointer;font-weight:800}
    .btn-ghost{background:transparent;border:1px solid rgba(255,255,255,0.18);color:#fff}
    .btn-primary{background:var(--gold);color:#000}
    /* grid */
    .layout{display:grid;grid-template-columns:300px 1fr 320px;gap:16px;margin-top:16px}
    @media(max-width:1100px){.layout{grid-template-columns:1fr;}.right{order:3}}
    /* sidebar */
    .sidebar{background:var(--card);border-radius:12px;padding:12px;box-shadow:0 6px 18px rgba(12,37,77,0.03)}
    .sidebar h4{margin:6px 0 12px;color:var(--ksu-dark)}
    .side-item{padding:10px;border-radius:10px;cursor:pointer;color:var(--ksu-dark);display:flex;justify-content:space-between;align-items:center}
    .side-item:hover{background:#f1f8ff}
    .col-list{display:grid;gap:8px;margin-top:10px}
    /* main */
    .main{min-height:360px}
    .hero{background:linear-gradient(180deg,#ffffff, #fbfdff);border-radius:12px;padding:18px;display:flex;gap:16px;align-items:center;box-shadow:0 6px 18px rgba(12,37,77,0.03)}
    .hero-left{flex:1}
    .hero h1{margin:0;color:var(--ksu-dark);font-size:22px}
    .lead{color:var(--muted);margin-top:6px}
    .hero-right{width:260px}
    .kpi{display:flex;gap:8px;margin-top:12px}
    .kpi .item{background:#f1f8ff;border-radius:8px;padding:10px;text-align:center;flex:1;color:var(--ksu-dark)}
    /* cards */
    .card{background:var(--card);border-radius:12px;padding:14px;box-shadow:0 6px 18px rgba(12,37,77,0.03);margin-top:14px}
    .card-title{font-weight:900;color:var(--ksu-dark);margin-bottom:8px}
    .service-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
    @media(max-width:900px){.service-grid{grid-template-columns:repeat(1,1fr)}}
    .service{padding:12px;border-radius:10px;border:1px solid #eef6ff}
    .service strong{display:block;color:var(--ksu-dark);margin-bottom:6px}
    .muted{color:var(--muted);font-size:14px}
    /* right panel */
    .right{position:sticky;top:20px}
    .contact{display:flex;gap:8px;align-items:center}
    .contact a{display:inline-block;padding:10px 12px;border-radius:10px;text-decoration:none;color:#000;background:#f1f7ff;border:1px solid #e3efff;font-weight:800}
    /* shop item */
    .product{display:flex;gap:10px;align-items:center;border-radius:10px;padding:10px;border:1px dashed #e6f1ff}
    .product img{width:72px;height:72px;border-radius:8px;object-fit:cover}
    /* form */
    form label{display:block;font-weight:800;margin-bottom:6px;color:var(--ksu-dark)}
    input,select,textarea{width:100%;padding:10px;border-radius:10px;border:1px solid #e6eefc;background:#fff}
    textarea{min-height:88px}
    .form-row{display:flex;gap:10px}
    .form-row > div{flex:1}
    .small{font-size:13px;color:var(--muted)}
    .note{background:#fff8e6;border-left:4px solid #ffd8a8;padding:10px;border-radius:8px;color:#6b4b00;margin-top:10px}
    /* footer */
    footer{margin-top:20px;text-align:center;color:var(--muted);font-size:13px;padding:18px}
    /* buttons inside */
    .btn-cta{background:var(--ksu-mid);color:#fff;padding:10px 12px;border-radius:10px;border:0;font-weight:900}
    .tag-plain{background:#eef7ff;padding:6px 8px;border-radius:8px;color:var(--ksu-dark);font-weight:800}
    .price{font-weight:900;color:var(--ksu-dark);font-size:18px}
    .link{color:var(--ksu-mid);font-weight:800;text-decoration:none}
    .quote{border-right:4px solid var(--ksu-mid);padding:10px;background:#f8fcff;border-radius:8px}
    .menu-buttons{display:flex;gap:8px;flex-wrap:wrap}
    .menu-buttons button{padding:8px 10px;border-radius:8px;border:1px solid #e8f4ff;background:#fff;cursor:pointer}
  </style>
</head>
<body>
  <div class="wrap">

    <!-- HEADER -->
    <header class="top" role="banner">
      <div class="logo">
        <div class="logo-box" aria-hidden="true">
          <!-- SVG Logo (Sanad + book) -->
          <svg width="48" height="48" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
            <rect x="0" y="0" width="64" height="64" rx="12" fill="#002b5c"/>
            <g transform="translate(8,10)" fill="#fff">
              <path d="M8 4h20v3H8zM0 10h28v3H0z" opacity="0.95"/>
              <path d="M4 20c0-4 6-6 10-6s10 2 10 6v10H4V20z" />
            </g>
          </svg>
        </div>
        <div>
          <div class="brand">منصة سند</div>
          <div class="tag">الخدمات الإلكترونية والتعليمية — جامعة الملك سعود</div>
        </div>
      </div>

      <div class="nav-actions">
        <a class="btn btn-ghost" href="#services" onclick="navTo('services')">الخدمات</a>
        <a class="btn btn-ghost" href="#colleges" onclick="navTo('colleges')">الكليات</a>
        <a class="btn btn-ghost" href="#shop" onclick="navTo('shop')">المتجر</a>
        <a class="btn btn-primary" href="#order" onclick="navTo('order')">اطلب خدمة</a>
      </div>
    </header>

    <!-- LAYOUT: sidebar / main / right -->
    <div class="layout">

      <!-- SIDEBAR -->
      <aside class="sidebar" aria-label="تنقّل سريع">
        <h4>تنقّل سريع</h4>

        <div class="side-item" onclick="navTo('services')">
          <div>الخدمات المتوفرة</div><div class="small">واجبات • مشاريع • ملخصات</div>
        </div>
        <div class="side-item" onclick="navTo('shared')">
          <div>المواد المشتركة</div><div class="small">نهج، فجب، تقن، ريد، إنجل، احصاء</div>
        </div>
        <div class="side-item" onclick="navTo('shop')">
          <div>متجر الملخصات</div><div class="small">ملفات جاهزة للميد والفاينل</div>
        </div>

        <hr style="border:none;border-top:1px solid #eef6ff;margin:12px 0">

        <h4>الكليات والمسارات</h4>
        <div class="col-list" id="collegeLinks">
          <!-- populated by JS -->
        </div>

        <hr style="border:none;border-top:1px solid #eef6ff;margin:12px 0">
        <div class="small">روابط مفيدة</div>
        <a class="link" href="https://t.me/Helping_KSU" target="_blank">قناة Helping_KSU</a><br/>
        <a class="link" href="https://t.me/KSUPDFbot" target="_blank">بوت الكتب KSUPDFbot</a>
      </aside>

      <!-- MAIN -->
      <main class="main">
        <!-- HERO -->
        <section class="hero" id="home">
          <div class="hero-left">
            <h1>خدمات طلابية متكاملة — منصة سند</h1>
            <div class="lead">حلول واجبات، كويزات، مشاريع، عروض وملخصات — متابعة خاصة حتى نهاية الترم. عمل خاص لكل طالب وحرص على الجودة ومقابل رسمي ومناسب.</div>

            <div class="kpi">
              <div class="item"><div class="tag-plain">خصوصية</div><div class="small">كل طالب له حل خاص</div></div>
              <div class="item"><div class="tag-plain">تسليم 12-24س</div><div class="small">الطلبات العاجلة ضمن الإمكانيات</div></div>
              <div class="item"><div class="tag-plain">دعم</div><div class="small">متابعة حتى نهاية الترم</div></div>
            </div>
          </div>

          <div class="hero-right">
            <div style="text-align:center;margin-bottom:10px"><strong class="price">بيانات الدفع الرسمية</strong></div>
            <div class="card" style="padding:10px">
              <div class="small">البنك: <strong>البنك العربي الوطني (anb)</strong></div>
              <div class="small">اسم المستفيد: <strong>عزام عبدالله عبدالعزيز ناجي</strong></div>
              <div class="small">رقم الحساب: <code>942000177167245</code></div>
              <div class="small">الآيبان: <code>SA0530100942000177167245</code></div>
              <div style="margin-top:8px">
                <a class="contact" href="https://wa.me/966565885750" target="_blank"><span class="btn">واتساب</span></a>
                <a class="contact" href="https://t.me/iTx7llxb_15" target="_blank"><span class="btn">تيليجرام</span></a>
              </div>
              <div class="small" style="margin-top:8px">بعد التحويل: أرسل إيصال الدفع على الواتساب ليتم تفعيل الطلب خلال وقت قصير.</div>
            </div>
          </div>
        </section>

        <!-- Services -->
        <section id="services" class="card">
          <div class="card-title">وش نقدّم؟ — الخدمات الرئيسية</div>
          <div class="small">نخدم كل المواد والتخصصات في جامعة الملك سعود (مسارات التحضيري + التخصصات)، وهذه نبذة مفصّلة لكل خدمة:</div>

          <div class="service-grid" style="margin-top:12px">
            <div class="service">
              <strong>حل واجبات & كويزات</strong>
              <div class="muted">حل سريع ومضبوط حسب متطلبات الدكتور. نضمن الدقة والخصوصية (حل خاص لكل طالب).</div>
              <div class="small" style="margin-top:8px">الوقت المعتاد: 12-24 ساعة (حسب التعقيد). السعر يبدأ 50 ر.س للكويز البسيط.</div>
            </div>

            <div class="service">
              <strong>مشاريع وتقارير وبحوث</strong>
              <div class="muted">كتابة متكاملة (محتوى، تنسيق، ملاحق، توثيق مراجع APA7 إذا طلب).</div>
              <div class="small" style="margin-top:8px">تسليم خلال 24 ساعة إلى 3 أيام حسب حجم المشروع. أسعار حسب متطلبات المشروع.</div>
            </div>

            <div class="service">
              <strong>عروض بوربوينت احترافية</strong>
              <div class="muted">تصميم شرائح متناسقة، جاهزة للعرض، مع ملاحظات المتحدث إن رغبت.</div>
              <div class="small" style="margin-top:8px">سعر العرض يبدأ 60 ر.س (حسب عدد الشرائح والتصميم).</div>
            </div>

            <div class="service">
              <strong>خريطة ذهنية / ملخصات</strong>
              <div class="muted">ملخصات وملازم مفهرسة للميد والفاينل — مرفقة بتجميعات ونماذج اختبارات.</div>
              <div class="small" style="margin-top:8px">ملزمة المادة تكون بأسعار تبدأ 30 ر.س — اشتراكات متاحة لتزويد كامل الفصل.</div>
            </div>

            <div class="service">
              <strong>اشتراك فصلي شامل (متابعة)</strong>
              <div class="muted">متابعة كاملة لكل الأعمال الفصلية + ملخصات محدثة + مراجعات قبل الميد والفاينل.</div>
              <div class="small" style="margin-top:8px">سعر اشتراك التحضيري: <strong>180 ر.س للمادة</strong> — خصم 15% عند الاشتراك في مادتين فأكثر.</div>
            </div>

            <div class="service">
              <strong>خدمات استشارية ورفع نسبة الاقتباس</strong>
              <div class="muted">نضمن أعمالًا خاصة ومراجعة لتقليل نسبة الاقتباس. ننبه عن مخاطر النسخ والذكاء الاصطناعي.</div>
            </div>
          </div>
        </section>

        <!-- Shared subjects (prices fixed for shared materials) -->
        <section id="shared" class="card">
          <div class="card-title">المواد المشتركة — مقترحات الأسعار</div>
          <div class="small">هنا أسعار نمطية للخدمات الخاصة بالمواد المشتركة بين المسارات (الأسعار تقريبية وتُؤكّد بعد إرسال تفاصيل المهمة).</div>

          <div style="margin-top:10px">
            <div class="product" style="justify-content:space-between">
              <div>
                <strong>نهج 101 — (التكليف البحثي / العرض / الخريطة)</strong>
                <div class="small">التكليف البحثي (توثيق مراجع APA): 50 ر.س — العرض التقديمي: 60 ر.س — الخريطة الذهنية: 40 ر.س</div>
              </div>
              <div style="text-align:center">
                <div class="price">حزمة 3× = 100 ر.س</div>
                <div class="small">وفر مع الحزمة</div>
              </div>
            </div>

            <div class="product" style="justify-content:space-between;margin-top:8px">
              <div>
                <strong>فجب 101 — مشاريع اللياقة</strong>
                <div class="small">مشروع قياسات / دراسة حالة / بحث: يبدأ من 60 ر.س للتكليف البسيط.</div>
              </div>
              <div style="text-align:center"><div class="price">عرض مخصص</div></div>
            </div>

            <div class="product" style="justify-content:space-between;margin-top:8px">
              <div>
                <strong>تقن 101 — مهارات الحاسب</strong>
                <div class="small">نماذج مشاريع (Word/Excel/Presentation) — الأسعار تبدأ 60 ر.س.</div>
              </div>
              <div style="text-align:center"><div class="price">ابدأ بـ60 ر.س</div></div>
            </div>

            <div class="product" style="justify-content:space-between;margin-top:8px">
              <div>
                <strong>ريد 101 — ريادة الأعمال</strong>
                <div class="small">مشروع دراسة جدوى: يبدأ من 80 ر.س (يشمل خطة تسويقية ومالية مختصرة).</div>
              </div>
              <div style="text-align:center"><div class="price">من 80 ر.س</div></div>
            </div>

            <div class="product" style="justify-content:space-between;margin-top:8px">
              <div>
                <strong>إنجل — مشروع CA</strong>
                <div class="small">المشروع CA: يتضمن نصوص وتصحيح ومراجعة — الأسعار تبدأ 50 ر.س.</div>
              </div>
              <div style="text-align:center"><div class="price">من 50 ر.س</div></div>
            </div>

            <div class="product" style="justify-content:space-between;margin-top:8px">
              <div>
                <strong>إحصاء — بنوك التمارين</strong>
                <div class="small">تجميع بنك أسئلة + حلول: 95 ر.س (يوصل خلال 24 ساعة بعد التحويل).</div>
              </div>
              <div style="text-align:center"><div class="price">95 ر.س</div></div>
            </div>
          </div>
        </section>

        <!-- Colleges / Guide -->
        <section id="colleges" class="card">
          <div class="card-title">دليل الكليات والتخصصات — KSU (مختصر)</div>
          <div class="small">اختر كليتك ثم التخصص لتظهر لك الخدمات المتاحة وزر "اطلب خدمة" يملأ النموذج تلقائيًا.</div>

          <div id="guideBoxes" style="margin-top:12px;display:grid;grid-template-columns:repeat(2,1fr);gap:12px">
            <!-- populated by JS -->
          </div>
        </section>

        <!-- Shop -->
        <section id="shop" class="card">
          <div class="card-title">متجر الملخصات والملازم</div>
          <div class="small">ملفات جاهزة للميد والفاينل — يتم إرسال الملف بعد تأكيد الدفع.</div>

          <div style="margin-top:12px">
            <div class="product">
              <img src="https://i.imgur.com/7XqQw7Y.png" alt="ملزمة">
              <div style="flex:1">
                <strong>ملزمة تحضيري — نهج 101 (تجميع + ملخص)</strong>
                <div class="small">ملخص مفهرس وجاهز للمذاكرة</div>
                <div style="margin-top:8px"><span class="price">30 ر.س</span></div>
              </div>
              <div>
                <button class="btn-cta" onclick="addToShop('ملزمة نهج 101',30)">أضف للسلة</button>
              </div>
            </div>

            <div style="margin-top:10px" id="cartArea" class="small hidden">السلة: <span id="cartCount">0</span> منتجات — الإجمالي: <strong id="cartTotal">0 ر.س</strong></div>
          </div>
        </section>

        <!-- Order form -->
        <section id="order" class="card">
          <div class="card-title">نموذج طلب خدمة — املأ البيانات</div>
          <div class="small">علشان نبدأ بسرعة: اكتب البيانات الأساسية واضغط "أرسل طلب" لفتح رسالة جاهزة على واتساب — بعد النقل والايصال نبدأ العمل.</div>

          <form id="requestForm" onsubmit="return submitRequest(event)" style="margin-top:12px">
            <div class="form-row">
              <div>
                <label>الاسم الكامل</label>
                <input id="f_name" placeholder="مثال: محمد عبدالله" required>
              </div>
              <div>
                <label>الرقم الجامعي (إن وُجد)</label>
                <input id="f_id" placeholder="مثال: 12345678">
              </div>
            </div>

            <div style="margin-top:10px">
              <label>الكلية / التخصص</label>
              <input id="f_college" placeholder="اختر الكلية من الدليل أو اكتبها" required>
            </div>

            <div class="form-row" style="margin-top:10px">
              <div>
                <label>المقرر / المادة</label>
                <input id="f_course" placeholder="مثال: نهج 101" required>
              </div>
              <div>
                <label>نوع الطلب</label>
                <select id="f_type" onchange="calcEstimate()" required>
                  <option value="">اختر نوع الخدمة</option>
                  <option value="واجب">حل واجب / كويز</option>
                  <option value="مشروع">مشروع / بحث</option>
                  <option value="عرض">عرض بوربوينت</option>
                  <option value="خريطة">خريطة ذهنية</option>
                  <option value="ملزمة">ملزمة / ملخص</option>
                  <option value="اشتراك">اشتراك فصلي (متابعة)</option>
                </select>
              </div>
            </div>

            <div style="margin-top:10px">
              <label>تفاصيل الطلب (مهم)</label>
              <textarea id="f_desc" placeholder="ملاحظات عن المطلوب، ملاحظات الدكتور، وقت التسليم المطلوب..."></textarea>
            </div>

            <div style="margin-top:10px">
              <label>إرفاق ملف (اختياري)</label>
              <input type="file" id="f_file">
              <div class="small">أرفع ملفات المقرر أو صور الأسئلة أو أي ملاحظة لتسريع التنفيذ.</div>
            </div>

            <div class="form-row" style="margin-top:10px">
              <div>
                <label>طريقة الدفع المفضلة</label>
                <select id="f_pay" onchange="calcEstimate()">
                  <option value="bank">تحويل بنكي / STC Pay</option>
                  <option value="card">بطاقة بنكية (Visa/Master)</option>
                  <option value="later">أقساط / اتفاق</option>
                </select>
              </div>
              <div>
                <label>عدد المواد (في حال اشتراك)</label>
                <input id="f_count" type="number" min="1" value="1" onchange="calcEstimate()">
              </div>
            </div>

            <div class="card" style="margin-top:12px;padding:10px">
              <div style="display:flex;justify-content:space-between;align-items:center">
                <div class="small">التكلفة التقديرية</div>
                <div id="f_estimate" class="price">0 ر.س</div>
              </div>
              <div class="small" style="margin-top:8px">السعر النهائي يتحدد بعد مراجعة التفاصيل. تأكيد الطلب يتم بعد استلام إيصال الدفع.</div>
            </div>

            <div style="margin-top:12px;display:flex;gap:8px;flex-wrap:wrap">
              <button class="btn-cta" type="submit">أرسل طلب — افتح واتساب</button>
              <button type="button" class="btn" onclick="resetForm()">مسح النموذج</button>
            </div>
          </form>

          <div style="margin-top:10px" class="note">
            <strong>تنبيه مهم:</strong> كل طالب له حل خاص. لا ننشر أو نشارك العمل في القروبات. لأي محاولة نسخ/مشاركة قد نطلب تعديلات أو نرفض العمل إذا كان مكررًا.
          </div>
        </section>

        <!-- For collaborators -->
        <section id="partners" class="card">
          <div class="card-title">انضم لفريق منصة سند — للمتعاونين والمحاضرين</div>
          <div class="small">لو أنت تدرس مادة، أو تصمم ملخصات، أو تقدر تشرح وتشتغل معنا كمُعاون — هذا النموذج لإرسال بياناتك وسنعاود التواصل.</div>

          <form id="partnerForm" onsubmit="return submitPartner(event)" style="margin-top:12px">
            <div class="form-row">
              <div>
                <label>الاسم</label>
                <input id="p_name" required placeholder="اسمك الكامل">
              </div>
              <div>
                <label>التخصص / المادة</label>
                <input id="p_field" required placeholder="مثال: محاضر في الإحصاء / مصمم ملخصات نهج">
              </div>
            </div>

            <div style="margin-top:10px">
              <label>لصق رابط تجريبي (شرح فيديو / نموذج عمل)</label>
              <input id="p_demo" placeholder="رابط يوتيوب أو تيليجرام">
            </div>

            <div style="margin-top:10px">
              <label>نبذة قصيرة عنك</label>
              <textarea id="p_bio" placeholder="خبرة، سنوات، أي شهادات"></textarea>
            </div>

            <div style="margin-top:10px">
              <button class="btn-cta" type="submit">أرسل طلب انضمام</button>
            </div>
          </form>
        </section>

        <!-- Terms & policies -->
        <section id="policy" class="card">
          <div class="card-title">سياسة العمل وحقوق الملكية</div>
          <div class="small">
            - كل الأعمال تُجهّز مخصصة لكل طالب. عند توفر مراجع خارجية نراعي التوثيق حسب نظام الجامعة.<br/>
            - يُحظر استخدام نسخ ولصق أو رفع نسبة الاقتباس > 25%، وننصح بالالتزام بقواعد الاقتباس.<br/>
            - نحتفظ بحق تعديل سياسات الدفع أو الأسعار بعد إشعار مسبق.<br/>
            - حقوق الأعمال: يتم تسليم العمل للطالب، ويمكن للمنصة الاحتفاظ بنسخة لأغراض تحسين الجودة والضمان.
          </div>
        </section>

      </main>

      <!-- RIGHT PANEL -->
      <aside class="right">
        <div class="card">
          <div style="display:flex;justify-content:space-between;align-items:center">
            <div>
              <div class="small">تواصل سريع</div>
              <div style="font-weight:900;color:var(--ksu-dark);margin-top:6px">خدمة العملاء — منصة سند</div>
            </div>
          </div>

          <div style="margin-top:12px">
            <a class="contact" href="https://wa.me/966565885750" target="_blank">📱 واتساب</a>
            <a class="contact" href="https://t.me/iTx7llxb_15" target="_blank">✉️ تيليجرام</a>
            <a class="contact" href="https://t.me/Helping_KSU" target="_blank">📚 قناة</a>
          </div>

          <div style="margin-top:12px" class="small">
            ⏰ ساعات العمل: يوميًا 10ص — 12ص<br/>
            ⚠️ نحن نرد الأفضل أولًا؛ الرجاء إرسال (اشتراك + اسم المقرر) أو ملخص طلبك مباشرة.
          </div>
        </div>

        <div class="card" style="margin-top:12px">
          <div class="card-title">لماذا تختارنا؟</div>
          <ul class="small">
            <li>كادر متخصص وتجارب سابقة ناجحة.</li>
            <li>عمل خاص لكل طالب — لا نسخ/لصق.</li>
            <li>متابعة حتى التأكد من قبول العمل.</li>
            <li>خيارات دفع مرنة وموثوقة.</li>
          </ul>
        </div>

        <div class="card" style="margin-top:12px">
          <div class="card-title">بيانات التحويل (للدفع اليدوي)</div>
          <div class="small">
            <strong>البنك:</strong> البنك العربي الوطني السعودي (anb) <br/>
            <strong>اسم المستفيد:</strong> عزام عبدالله عبدالعزيز ناجي <br/>
            <strong>رقم الحساب:</strong> <code>942000177167245</code> <br/>
            <strong>الآيبان:</strong> <code>SA0530100942000177167245</code>
          </div>
          <div class="small" style="margin-top:8px">للمستخدمين في بنوك أخرى (راجحي / الأهلي) يكفي لصق الآيبان وتحويل المبلغ — أرسل الإيصال فورًا على الواتساب.</div>
        </div>
      </aside>

    </div> <!-- /layout -->

    <footer>
      © منصة سند للخدمات الإلكترونية والتعليمية — جامعة الملك سعود KSU • جميع الحقوق محفوظة.
    </footer>
  </div>

  <!-- SCRIPT: data + interaction -->
  <script>
    /* ===== بيانات دليل الكليات (موجز من المحتوى الذي طلبته) ===== */
    const GUIDE = {
      "المسار الصحي": {
        "كلية الطب": ["طب وجراحة"],
        "كلية طب الأسنان": ["طب أسنان"],
        "كلية الصيدلة": ["دكتور صيدلة"],
        "العلوم الطبية التطبيقية": ["تغذية سريرية","مختبرات","علاج طبيعي","أشعة","تنفس","بصريات"],
        "كلية التمريض": ["تمريض عام"],
        "كلية الخدمات الطبية الطارئة": ["الخدمات الطبية الطارئة"]
      },
      "المسار العلمي": {
        "كلية الهندسة": ["مدني","كهربائي","ميكانيكي","كيميائي","بترول","مساحة"],
        "علوم الحاسب والمعلومات": ["علوم الحاسب","هندسة البرمجيات","نظم المعلومات"],
        "كلية العلوم": ["رياضيات","فيزياء","كيمياء","أحياء","إحصاء"],
        "كلية الأغذية والزراعة": ["إنتاج نباتي","إنتاج حيواني","علوم أغذية"]
      },
      "مسار إدارة الأعمال": {
        "كلية إدارة الأعمال": ["محاسبة","مالية","تسويق","نظم معلومات إدارية","إدارة","اقتصاد"]
      },
      "المسار الإنساني": {
        "الآداب": ["لغة عربية","إعلام","تاريخ","جغرافيا","علم اجتماع"],
        "الحقوق والدراسات الإسلامية": ["حقوق","شريعة"],
        "اللغات والترجمة": ["إنجليزي","فرنسي","صيني"]
      },
      "فروع": {
        "المزاحمية": ["هندسة تطبيقية","علوم حاسب تطبيقية","إدارة أعمال تطبيقية"]
      }
    };

    /* Populate college links (sidebar & guideBoxes) */
    const collegeLinks = document.getElementById('collegeLinks');
    const guideBoxes = document.getElementById('guideBoxes');
    for(const track in GUIDE){
      const div = document.createElement('div');
      div.className = 'side-item';
      div.innerHTML = `<div>${track}</div><div class="small">فتح</div>`;
      div.onclick = ()=> showTrack(track);
      collegeLinks.appendChild(div);

      // guide box
      const box = document.createElement('div');
      box.style.border='1px solid #eef6ff';
      box.style.padding='12px';
      box.style.borderRadius='10px';
      box.innerHTML = `<strong style="color:var(--ksu-dark)">${track}</strong><div class="small" style="margin-top:8px">${Object.keys(GUIDE[track]).join(' • ')}</div>
        <div style="margin-top:8px"><button class="btn" onclick="showTrack('${escapeJS(track)}')">عرض التخصّصات</button></div>`;
      guideBoxes.appendChild(box);
    }

    function escapeJS(s){ return s.replace(/'/g,"\\'") };

    /* Show track -> list colleges & special buttons */
    function showTrack(track){
      const colleges = GUIDE[track];
      let html = `<div class="card-title">${track} — الكليات</div><div style="margin-top:8px" class="small">اختر الكلية لعرض التخصصات والخدمات المتاحة.</div><div style="margin-top:10px;display:grid;gap:10px">`;
      for(const col in colleges){
        html += `<div style="padding:10px;border-radius:10px;border:1px solid #eef6ff">
          <strong style="color:var(--ksu-dark)">${col}</strong>
          <div class="small" style="margin-top:6px">${colleges[col].join(' • ')}</div>
          <div style="margin-top:8px">
            <button class="btn" onclick="prefillCollege('${escapeJS(col)}')">أطلب من هنا</button>
            <button class="btn" onclick="showCollege('${escapeJS(col)}')">عرض خدمات الكلية</button>
          </div>
        </div>`;
      }
      html += `</div>`;
      openDynamic(html);
    }

    /* show college detail with services */
    function showCollege(col){
      let html = `<div class="card-title">خدمات كلية ${col}</div>
        <div class="small">نقدم: حل الكويزات/الواجبات، مشاريع، عروض، ملخصات، اشتراكات متابعة.</div>
        <div style="margin-top:12px;display:grid;gap:8px">
          <div style="padding:10px;border-radius:8px;border:1px solid #eef6ff">
            <strong>حل واجبات/كويز</strong>
            <div class="small">سريع وخاص — يبدأ من 50 ر.س</div>
            <div style="margin-top:6px"><button class="btn" onclick="prefillService('${escapeJS(col)}','واجب')">اطلب حل واجب</button></div>
          </div>

          <div style="padding:10px;border-radius:8px;border:1px solid #eef6ff">
            <strong>مشروع/بحث/تقرير</strong>
            <div class="small">تنسيق كامل + ملاحق + توثيق — السعر يتحدد حسب متطلبات المشروع.</div>
            <div style="margin-top:6px"><button class="btn" onclick="prefillService('${escapeJS(col)}','مشروع')">اطلب مشروع</button></div>
          </div>

          <div style="padding:10px;border-radius:8px;border:1px solid #eef6ff">
            <strong>اشتراك متابعة للمقرر</strong>
            <div class="small">180 ر.س للمادة (خصم 15% للمادتين أو أكثر)</div>
            <div style="margin-top:6px"><button class="btn" onclick="prefillService('${escapeJS(col)}','اشتراك')">اشترك الآن</button></div>
          </div>
        </div>`;
      openDynamic(html);
    }

    /* dynamic panel overlay (use simple modal-like area) */
    function openDynamic(html){
      // locate or create an area at top of main
      let panel = document.getElementById('dynamicPanel');
      if(!panel){
        panel = document.createElement('div');
        panel.id = 'dynamicPanel';
        panel.className = 'card';
        document.querySelector('.main').prepend(panel);
      }
      panel.innerHTML = html;
      panel.scrollIntoView({behavior:'smooth'});
    }

    /* prefill functions */
    function prefillCollege(col){
      document.getElementById('f_college').value = col;
      navTo('order');
      focusField('f_course');
    }
    function prefillService(col,svc){
      document.getElementById('f_college').value = col;
      document.getElementById('f_type').value = svc;
      if(svc==='واجب') document.getElementById('f_course').value = 'واجب المقرر';
      if(svc==='مشروع') document.getElementById('f_course').value = 'مشروع المقرر';
      if(svc==='اشتراك') document.getElementById('f_course').value = 'اشتراك متابعة للمقرر';
      calcEstimate();
      navTo('order');
      focusField('f_desc');
    }
    function focusField(id){ setTimeout(()=>{ const el=document.getElementById(id); if(el) el.focus(); },300) }

    /* shop cart */
    let CART = [];
    function addToShop(name,price){
      CART.push({name,price});
      updateCartUI();
      alert('تم إضافة المنتج للسلة — افتح السلة أسفل المتجر لإرسال الطلب');
    }
    function updateCartUI(){
      const area = document.getElementById('cartArea');
      const count = document.getElementById('cartCount');
      const total = document.getElementById('cartTotal');
      if(CART.length===0){ area.classList.add('hidden'); return; }
      area.classList.remove('hidden');
      const sum = CART.reduce((s,p)=>s+p.price,0);
      count.innerText = CART.length;
      total.innerText = sum + ' ر.س';
    }

    /* estimate logic for order form */
    function calcEstimate(){
      const type = document.getElementById('f_type').value;
      const count = parseInt(document.getElementById('f_count').value||1,10);
      let val = 0;
      if(type==='واجب') val = 50;
      else if(type==='مشروع') val = 120;
      else if(type==='عرض') val = 60;
      else if(type==='خريطة') val = 40;
      else if(type==='ملزمة') val = 35;
      else if(type==='اشتراك'){ val = 180 * count; if(count>=2) val = Math.round(val * 0.85); }
      // include cart
      const cartSum = CART.reduce((s,p)=>s+p.price,0);
      val += cartSum;
      document.getElementById('f_estimate').innerText = val + ' ر.س';
      return val;
    }

    /* submit request -> open WhatsApp message */
    function submitRequest(e){
      e.preventDefault();
      const name = document.getElementById('f_name').value.trim() || '-';
      const id = document.getElementById('f_id').value.trim() || '-';
      const college = document.getElementById('f_college').value.trim() || '-';
      const course = document.getElementById('f_course').value.trim() || '-';
      const type = document.getElementById('f_type').value || '-';
      const desc = document.getElementById('f_desc').value.trim() || '-';
      const pay = document.getElementById('f_pay').value;
      const count = document.getElementById('f_count').value || 1;
      const estimate = calcEstimate();
      const fileInput = document.getElementById('f_file');
      const fileName = (fileInput && fileInput.files && fileInput.files[0]) ? fileInput.files[0].name : 'لا يوجد';

      let msg = `🟢 طلب خدمة — منصة سند\n`;
      msg += `الاسم: ${name}\n`;
      msg += `الرقم الجامعي: ${id}\n`;
      msg += `الكلية/التخصص: ${college}\n`;
      msg += `المقرر: ${course}\n`;
      msg += `نوع الخدمة: ${type}\n`;
      msg += `تفاصيل: ${desc}\n`;
      msg += `عدد مواد (إن اشتراك): ${count}\n`;
      msg += `طريقة الدفع: ${pay}\n`;
      msg += `تقدير السعر: ${estimate} ر.س\n`;
      msg += `ملف مرفق: ${fileName}\n\n`;
      msg += `*بعد التحويل:* أرسل إيصال الدفع على هذا الرقم لتأكيد الطلب وبدء التنفيذ (نبدأ بعد تأكيد الإيصال).`;

      const wa = 'https://wa.me/966565885750?text=' + encodeURIComponent(msg);
      window.open(wa,'_blank');
      alert('تم تجهيز رسالة الطلب — سيفتح واتساب لإرسالها. بعد استلام الإيصال نبدأ العمل فورًا.');
      return false;
    }

    /* partner form */
    function submitPartner(e){
      e.preventDefault();
      const name = document.getElementById('p_name').value.trim();
      const field = document.getElementById('p_field').value.trim();
      const demo = document.getElementById('p_demo').value.trim() || '-';
      const bio = document.getElementById('p_bio').value.trim() || '-';

      let msg = `📩 طلب شراكة — منصة سند\nالاسم: ${name}\nالتخصص: ${field}\nرابط تجريبي: ${demo}\nنبذة: ${bio}\n\n`;
      msg += 'نرجو إرسال هذه الرسالة عبر الواتساب للنظر في الانضمام.';
      const wa = 'https://wa.me/966565885750?text=' + encodeURIComponent(msg);
      window.open(wa,'_blank');
      alert('تم تجهيز رسالة الشراكة — افتح واتساب لإرسالها.');
      return false;
    }

    /* reset form */
    function resetForm(){
      document.getElementById('requestForm').reset();
      document.getElementById('f_estimate').innerText = '0 ر.س';
    }

    /* nav helper */
    function navTo(id){
      const el = document.getElementById(id);
      if(el) el.scrollIntoView({behavior:'smooth'});
    }

    /* init: populate some sidebar quick links */
    (function init(){
      // show top message or latest published
      // attach approximate estimate updater
      document.getElementById('f_type').addEventListener('change',calcEstimate);
      document.getElementById('f_count').addEventListener('change',calcEstimate);
      // initial populate dynamic panel placeholder
      // (nothing else)
    })();
  </script>
</body>
</html>
