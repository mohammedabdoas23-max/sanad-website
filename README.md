<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>منصة سند — خدمات طلابية إلكترونية وتعليمية</title>
  <meta name="description" content="منصة سند للخدمات الطلابية — ملخصات، حلول واجبات، مشاريع، باقات، متجر. دعم لطلاب جامعة الملك سعود KSU."/>
  <style>
    /* ---------- Base & Fonts ---------- */
    :root{
      --ksu-blue:#002b5c;
      --accent:#0066cc;
      --muted:#6b7280;
      --card:#ffffff;
      --bg:#f6f8fb;
      --gold:#ffb700;
      --success:#16a34a;
      --danger:#ef4444;
    }
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, "Segoe UI", Tahoma, Arial; background:var(--bg); color:#0f172a; line-height:1.55}
    a{text-decoration:none;color:inherit}
    .container{max-width:1150px;margin:0 auto;padding:22px}

    /* ---------- Header ---------- */
    header{background:linear-gradient(90deg,var(--ksu-blue),#004aad);color:#fff;padding:18px 0;box-shadow:0 6px 24px rgba(2,6,23,0.12)}
    .brand{display:flex;gap:14px;align-items:center}
    .logo{width:54px;height:54px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;padding:6px}
    .logo svg{width:40px;height:40px}
    header h1{font-size:18px;margin:0}
    nav{display:flex;gap:10px;align-items:center;margin-left:auto}
    nav a{color:rgba(255,255,255,0.95);padding:8px 12px;border-radius:8px;font-weight:600}
    nav a.cta{background:var(--gold);color:#000}

    /* ---------- Hero ---------- */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:26px;align-items:center;padding:36px 0}
    .hero .card{background:var(--card);padding:22px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.06)}
    .hero h2{color:var(--ksu-blue);margin:0 0 8px;font-size:26px}
    .lead{color:var(--muted);margin-bottom:14px}
    .features{display:flex;gap:10px;flex-wrap:wrap}
    .pill{background:#eef7ff;color:var(--accent);padding:8px 12px;border-radius:999px;font-weight:600;font-size:13px}

    /* ---------- Cards grid ---------- */
    .grid{display:grid;gap:16px}
    .cols-3{grid-template-columns:repeat(3,1fr)}
    .service-card{background:var(--card);padding:14px;border-radius:10px;border:1px solid #eef3ff}
    .service-card h3{margin:0 0 8px;color:var(--ksu-blue)}
    .muted{color:var(--muted);font-size:14px}

    /* ---------- Shop & products ---------- */
    .product{display:flex;gap:12px;align-items:center;padding:12px;border-radius:10px;border:1px dashed #e6eefc}
    .product img{width:64px;height:64px;border-radius:8px;object-fit:cover}
    .price{font-weight:800;color:var(--ksu-blue);}

    /* ---------- Form ---------- */
    form .row{display:flex;gap:10px;flex-wrap:wrap}
    label{font-weight:700;margin-bottom:6px;display:block;color:var(--ksu-blue)}
    input[type=text],input[type=email],select,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid #dbeafe;background:#fff}
    textarea{min-height:120px;resize:vertical}
    .small{font-size:13px;color:var(--muted)}

    /* ---------- Buttons ---------- */
    .btn{display:inline-block;padding:10px 14px;border-radius:10px;font-weight:700;cursor:pointer;border:0}
    .btn.primary{background:var(--accent);color:#fff}
    .btn.ghost{background:transparent;border:1px solid #dbeafe;color:var(--ksu-blue)}
    .btn.warn{background:var(--gold);color:#000}

    /* ---------- Modal / Panels ---------- */
    .panel{background:var(--card);padding:14px;border-radius:10px;border:1px solid #e6eefc}
    .right{padding-left:18px}

    /* ---------- Footer ---------- */
    footer{background:#061325;color:#cfe8ff;padding:22px;margin-top:26px;text-align:center;border-top:3px solid rgba(255,255,255,0.04)}
    footer a{color:#fff;font-weight:700}

    /* ---------- Responsive ---------- */
    @media(max-width:980px){
      .hero{grid-template-columns:1fr}
      nav{display:none}
      .cols-3{grid-template-columns:repeat(2,1fr)}
    }
    @media(max-width:560px){
      .cols-3{grid-template-columns:1fr}
    }

    /* ---------- Fancy touches ---------- */
    .tag{background:#e6f2ff;color:var(--accent);padding:6px 10px;border-radius:8px;font-weight:700}
    .note{background:#fff7ed;border-left:4px solid #ffd8a8;padding:10px;border-radius:8px;color:#5a3b00}
    .badge{background:var(--success);color:#fff;padding:6px 8px;border-radius:8px;font-weight:700}
    .inline{display:flex;gap:8px;align-items:center}
    .center{text-align:center}
  </style>
</head>
<body>

  <!-- HEADER -->
  <header>
    <div class="container" style="display:flex;align-items:center">
      <div class="brand">
        <div class="logo" aria-hidden="true">
          <!-- SVG logo (سند) -->
          <svg viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
            <rect x="2" y="2" width="60" height="60" rx="10" fill="#002b5c"/>
            <path d="M18 38c6-6 12-6 18 0" stroke="#fff" stroke-width="3" stroke-linecap="round" fill="none"/>
            <circle cx="23" cy="24" r="3" fill="#fff"/>
            <circle cx="35" cy="24" r="3" fill="#fff"/>
          </svg>
        </div>
        <div>
          <h1 style="font-size:18px;margin-bottom:2px">منصة سند</h1>
          <div style="font-size:13px;color:#dbeafc">خدمات إلكترونية وتعليمية — للطلاب</div>
        </div>
      </div>

      <nav aria-label="الرئيسية">
        <a href="#services">الخدمات</a>
        <a href="#packages">الباقات</a>
        <a href="#shop">المتجر</a>
        <a href="#guide">دليل KSU</a>
        <a href="#order" class="cta">اطلب خدمة</a>
      </nav>
    </div>
  </header>

  <!-- HERO -->
  <main class="container">
    <section class="hero">
      <div class="card">
        <h2>خدمات طلابية متكاملة لجامعة الملك سعود — سند</h2>
        <p class="lead">نقدّم لك حل الواجبات والكويزات، تنفيذ المشاريع والتقارير، تجهيز عروض بوربوينت، ملخصات ومراجعات مفهرسة — متابعين معك خطوة بخطوة لغاية تسليم العمل.</p>

        <div class="features">
          <span class="pill">متابعة خاصة</span>
          <span class="pill">تسليم خلال 12-24 ساعة</span>
          <span class="pill">حل مخصص لكل طالب</span>
          <span class="pill">دفع آمن — أقساط متاحة</span>
        </div>

        <div style="margin-top:16px">
          <a class="btn primary" href="#order">اطلب خدمة الآن</a>
          <a class="btn ghost" href="https://t.me/Helping_KSU" target="_blank">قناة المتجر</a>
        </div>

        <div style="margin-top:14px" class="small">
          <strong>المكان الموثوق:</strong> خدماتنا مجرّبة مع طلاب الأترام السابقة — كل عمل خاص مخصص لضمان القبول وتقليل الاقتباس.
        </div>
      </div>

      <aside class="panel right">
        <div class="center">
          <div style="font-size:13px;color:var(--muted)">سعر الاشتراك لطلاب السنة الأولى المشتركة</div>
          <div style="font-size:28px;font-weight:900;color:var(--ksu-blue)">180 ر.س / المادة</div>
          <div class="small" style="margin-top:6px">خصم 15% للمشترك بأكثر من مادة — السعر بعد الخصم: <strong id="subDiscount">153 ر.س</strong> للمادة</div>
          <div style="margin-top:12px" class="small">في حال تبي خيار اقتصادي بدون حضور المحاضرات: <strong>100 ر.س/مادة</strong></div>

          <div style="margin-top:14px">
            <a class="btn warn" href="#order">سجّل اشتراك</a>
          </div>
        </div>
      </aside>
    </section>

    <!-- SERVICES -->
    <section id="services" style="margin-top:18px">
      <h2>وش نقدّم؟</h2>
      <div class="grid cols-3" style="margin-top:12px">
        <div class="service-card">
          <h3>حل الواجبات & الكويزات</h3>
          <div class="muted">حل دقيق ومتابعة خاصة لكل طالب — نضمن قبول العمل.</div>
        </div>
        <div class="service-card">
          <h3>مشاريع وتقارير</h3>
          <div class="muted">تنفيذ كامل حسب متطلبات المقرر مع تسليم مرتب.</div>
        </div>
        <div class="service-card">
          <h3>عروض بوربوينت</h3>
          <div class="muted">تصميم احترافي جاهز للعرض بالجامعة.</div>
        </div>
        <div class="service-card">
          <h3>ملخصات ومذاكرات</h3>
          <div class="muted">ملخصات مفهرسة للـميد والفاينل وتجميعات مهمة.</div>
        </div>
        <div class="service-card">
          <h3>استشارات دراسية</h3>
          <div class="muted">نرتب لك خطة مذاكرة ومتابعة خاصة للوصول للدرجات المطلوبة.</div>
        </div>
        <div class="service-card">
          <h3>قنوات خاصة للمشتركين</h3>
          <div class="muted">قناة مخصصة لكل مقرر فيها الشروحات، الملخصات، والتسريبات المحلولة قبل الاختبار.</div>
        </div>
      </div>
    </section>

    <!-- PACKAGES -->
    <section id="packages" style="margin-top:20px">
      <h2>الباقات الشهيرة</h2>
      <div class="grid cols-3" style="margin-top:12px">
        <div class="card">
          <h3>باقة أساسي</h3>
          <div class="price">150 ر.س</div>
          <div class="small">حل واجب فردي + ملخص مختصر + تسليم سريع</div>
          <div style="margin-top:10px"><a class="btn primary" href="#order" onclick="prefillPackage('أساسي',150)">اطلب باقة</a></div>
        </div>
        <div class="card">
          <h3>باقة قياسي</h3>
          <div class="price">200 ر.س</div>
          <div class="small">حل واجبات + كويزات + ملخصات مفهرسة + متابعة</div>
          <div style="margin-top:10px"><a class="btn primary" href="#order" onclick="prefillPackage('قياسي',200)">اطلب باقة</a></div>
        </div>
        <div class="card">
          <h3>باقة بريميوم</h3>
          <div class="price">250 ر.س</div>
          <div class="small">حل شامل + مشاريع + قناة خاصة + دعم أولوية</div>
          <div style="margin-top:10px"><a class="btn primary" href="#order" onclick="prefillPackage('بريميوم',250)">اطلب باقة</a></div>
        </div>
      </div>
    </section>

    <!-- SHOP -->
    <section id="shop" style="margin-top:22px">
      <h2>المتجر — ملخصات وملازم</h2>
      <div class="small">مكاتب رقمية جاهزة للميد/فاينل — تقدر تشوف منتجاتنا في قناة المتجر أو تشتري مباشرة هنا.</div>

      <div style="margin-top:12px" class="grid">
        <!-- Example product -->
        <div class="product">
          <img src="https://i.imgur.com/7XqQw7Y.png" alt="ملزمة مثال">
          <div style="flex:1">
            <div style="display:flex;justify-content:space-between;align-items:center">
              <strong>ملزمة نهج 101 — تجميع شامل</strong>
              <div class="price">35 ر.س</div>
            </div>
            <div class="muted">ملخصات ومقاطع أسئلة مهمة للميد والفاينل</div>
            <div style="margin-top:8px">
              <a class="btn ghost" onclick="addToCart('ملزمة نهج 101',35)">أضف للسلة</a>
            </div>
          </div>
        </div>

        <!-- Add more products as needed -->
      </div>

      <div id="cartBox" style="margin-top:12px;display:none" class="card">
        <div style="display:flex;justify-content:space-between;align-items:center">
          <strong>سلة المشتريات</strong><span id="cartTotal">0 ر.س</span>
        </div>
        <div style="margin-top:10px">
          <a class="btn primary" href="#order" onclick="openCartOrder()">اكمال الدفع</a>
        </div>
      </div>
    </section>

    <!-- GUIDE KSU -->
    <section id="guide" style="margin-top:22px">
      <h2>دليل جامعة الملك سعود — ملخص المسارات & الكليات</h2>
      <div class="card">
        <details open>
          <summary>المسار الصحي 🏥</summary>
          <div class="small">كلية الطب • طب الأسنان • الصيدلة • العلوم الطبية التطبيقية (مختبرات، علاج طبيعي، تغذية، أشعة) • التمريض • الخدمات الطبية الطارئة</div>
        </details>
        <details>
          <summary>المسار العلمي ⚙️</summary>
          <div class="small">الهندسة (كل التخصصات) • علوم الحاسب • كلية العلوم (رياضيات، فيزياء، كيمياء، أحياء، إحصاء)</div>
        </details>
        <details>
          <summary>مسار إدارة الأعمال 💼</summary>
          <div class="small">المحاسبة • المالية • التسويق • نظم المعلومات الإدارية • الإدارة • الاقتصاد</div>
        </details>
        <details>
          <summary>المسار الإنساني ✨</summary>
          <div class="small">الآداب • التربية • الشريعة • الحقوق • اللغات والترجمة • السياحة والآثار • الفنون وعلوم الرياضة</div>
        </details>
      </div>
      <p class="small" style="margin-top:10px">روابط مفيدة: بوت الكتب والملخصات — <a href="https://t.me/KSUPDFbot" target="_blank">KSUPDFbot</a> · قناة المتجر — <a href="https://t.me/Helping_KSU" target="_blank">Helping_KSU</a></p>
    </section>

    <!-- ORDER FORM -->
    <section id="order" style="margin-top:22px">
      <h2>نموذج طلب خدمة — عبّ التفاصيل عشان نبدأ</h2>
      <div class="grid" style="grid-template-columns:1fr 380px;gap:18px">
        <div class="card">
          <form id="orderForm" onsubmit="return handleSubmit(event)">
            <div class="row">
              <div style="flex:1">
                <label>اسم الطالب / الطالبة</label>
                <input type="text" id="studentName" required placeholder="الاسم الكامل">
              </div>
              <div style="width:160px">
                <label>الرقم الجامعي</label>
                <input type="text" id="studentId" placeholder="مثال: 12345678">
              </div>
            </div>

            <div style="margin-top:10px">
              <label>الكلية / التخصص</label>
              <select id="major" required>
                <option value="">اختر الكلية أو المسار</option>
                <option>السنة الأولى المشتركة — نهج/فجب/تقن/انجل/ريد</option>
                <option>كلية الطب</option>
                <option>كلية الصيدلة</option>
                <option>كلية الهندسة</option>
                <option>كلية علوم الحاسب</option>
                <option>كلية إدارة الأعمال</option>
                <option>الآداب / الإنساني</option>
              </select>
            </div>

            <div style="margin-top:10px">
              <label>نوع الخدمة المطلوبة</label>
              <select id="serviceType" onchange="serviceChanged()" required>
                <option value="">اختر الخدمة</option>
                <option value="واجب">حل واجب / كويز</option>
                <option value="مشروع">مشروع / تقرير</option>
                <option value="عرض">عرض بوربوينت</option>
                <option value="ملزمة">ملازمة / ملخص</option>
                <option value="اشتراك">اشتراك ترم (متابعة كاملة)</option>
              </select>
            </div>

            <div id="serviceDetails" style="margin-top:10px;display:none">
              <label>تفاصيل الطلب (أذكر المادة، موعد التسليم، ملاحظات)</label>
              <textarea id="details" placeholder="مثال: مقرر نهج 101 - مشروع الخريطة - الجلسة 3 ..."></textarea>
              <div class="small" style="margin-top:6px">تقدر تضيف ملف أو صورة للواجب بعد ارسال الطلب — أو ارفقها هنا.</div>
            </div>

            <div style="margin-top:10px">
              <label>ارفق ملف (اختياري)</label>
              <input type="file" id="fileUpload" accept=".pdf,.doc,.docx,.zip,.png,.jpg">
              <div class="small">PDF/Word/Zip/صورة — مرفوع على جهازك وسيظهر اسم الملف في ملخص الطلب.</div>
            </div>

            <div style="margin-top:10px">
              <label>المنتجات أو المواد (إن وجدت)</label>
              <div class="small">اختر المواد المشتركة أو اضافات من المتجر:</div>
              <div style="display:flex;gap:8px;margin-top:8px;flex-wrap:wrap">
                <button type="button" class="btn ghost" onclick="toggleMaterial('نهج 101')">نهج 101</button>
                <button type="button" class="btn ghost" onclick="toggleMaterial('فجب 101')">فجب 101</button>
                <button type="button" class="btn ghost" onclick="toggleMaterial('تقن 101')">تقن 101</button>
                <button type="button" class="btn ghost" onclick="toggleMaterial('ريد 101')">ريد 101</button>
                <button type="button" class="btn ghost" onclick="toggleMaterial('انجل')">انجل</button>
                <button type="button" class="btn ghost" onclick="toggleMaterial('احصاء')">احصاء</button>
              </div>
            </div>

            <div style="margin-top:12px">
              <label>طريقة الدفع المفضلة</label>
              <select id="payMethod" onchange="payMethodChanged()">
                <option value="bank">التحويل البنكي / STC Pay</option>
                <option value="card">بطاقات (Visa / Master)</option>
                <option value="crypto">دفع بالعملات الرقمية</option>
                <option value="onreceive">الدفع بعد التسليم (اتفاق)</option>
              </select>
            </div>

            <div id="priceBox" style="margin-top:12px" class="panel">
              <div class="small">تفاصيل السعر التلقائية</div>
              <div style="display:flex;justify-content:space-between;align-items:center;margin-top:8px">
                <div>المجموع المتوقع:</div>
                <div style="font-weight:900;color:var(--ksu-blue)" id="calcTotal">0 ر.س</div>
              </div>
              <div style="margin-top:8px" class="small">(تأكيد السعر النهائي بعد إرسال تفاصيل الطلب والتحقق من المتطلبات)</div>
            </div>

            <div style="margin-top:12px;display:flex;gap:10px;align-items:center">
              <button type="submit" class="btn primary">إرسال الطلب & فتح واتساب</button>
              <button type="button" class="btn ghost" onclick="resetOrder()">مسح</button>
            </div>
          </form>
        </div>

        <!-- RIGHT PANEL -->
        <div class="panel">
          <h4>بيانات التحويل اليدوي</h4>
          <p class="small">
            <strong>البنك:</strong> البنك العربي الوطني السعودي (ANB)<br>
            <strong>اسم المستفيد:</strong> عزام عبدالله عبدالعزيز ناجي<br>
            <strong>رقم الحساب:</strong> <code>942000177167245</code><br>
            <strong>IBAN:</strong> <code>SA0530100942000177167245</code>
          </p>

          <div class="note" style="margin-top:10px">
            بعد التحويل أرسل إيصال الدفع هنا في الواتساب أو داخل البوت. الدفع بدون إيصال ما يتم اعتماده.
          </div>

          <h4 style="margin-top:12px">طرق أخرى</h4>
          <p class="small">لو عندك بنك ثاني (راجحي، الأهلي، ساب...) تقدر تحول برضه عبر الآيبان أعلاه من أي بنك.</p>

          <div style="margin-top:12px" class="inline">
            <a class="btn primary" href="https://wa.me/966565885750" target="_blank">راسلنا واتساب</a>
            <a class="btn ghost" href="https://t.me/iTx7llxb_15" target="_blank">تيليجرام</a>
          </div>
        </div>
      </div>
    </section>

    <!-- JOIN / Partners -->
    <section id="partners" style="margin-top:22px">
      <h2>انضم للفريق أو للأخصائيين</h2>
      <div class="card">
        <p class="small">لو أنت متخصص (محاضر، مترجم، مصمم ملخصات، مراجع أكاديمي) وحاب تضيف خدمتك في منصة سند، ارسل طلب انضمام مع تفاصيل خبرتك ورابط تجريبي للمحتوى. نفتح فرص تعاون بمقابل مالي أو نسبة.</p>
        <div style="margin-top:10px">
          <a class="btn primary" href="https://wa.me/966565885750?text=اريد%20انضم%20كمتخصص%20في%20منصة%20سند">انضم كمختص</a>
          <a class="btn ghost" href="mailto:contact@sanad.example?subject=انضمام%20مقدم%20خدمة">ابعت ايميل</a>
        </div>
      </div>
    </section>

    <!-- TERMS & NOTES -->
    <section style="margin-top:22px">
      <h2>تنبيهات وسياسة العمل</h2>
      <div class="card small">
        <ul>
          <li><strong>خصوصية ومصداقية:</strong> كل عمل يُجهَّز خصيصًا لكل طالب. أي عمل مكرر أو منسوخ قد يُرفض من قِبل الجامعة.</li>
          <li><strong>حظر النسخ العشوائي:</strong> لا تعتمد على النسخ واللصق ولا تعتمد اعتماد كامل على مولدات الذكاء الاصطناعي دون مراجعة بشرية.</li>
          <li><strong>التسليم:</strong> عادةً بين 12-24 ساعة حسب نوع الخدمة؛ المشاريع الكبيرة قد تحتاج وقتاً أطول — يتم توضيح الوقت عند تأكيد الطلب.</li>
          <li><strong>الضمان:</strong> نراجع العمل قبل التسليم ويكون مُصمم ليقبل لدى معظم الدكاترة (لكن قرار القبول النهائي بيد الجامعة والدكتور).</li>
        </ul>
      </div>
    </section>

  </main>

  <!-- FOOTER -->
  <footer>
    <div class="container">
      <div style="margin-bottom:8px">© منصة سند للخدمات الإلكترونية والتعليمية — جميع الحقوق محفوظة</div>
      <div class="small">قنوات التواصل: <a href="https://wa.me/966565885750">واتساب</a> • <a href="https://t.me/iTx7llxb_15">تيليجرام</a> • بوت الكتب: <a href="https://t.me/KSUPDFbot">KSUPDFbot</a></div>
    </div>
  </footer>

  <!-- ---------- SCRIPTS ---------- -->
  <script>
    // Simple cart & selected materials
    let cart = [];
    let selectedMaterials = new Set();
    const cartBox = document.getElementById('cartBox');
    const cartTotalEl = document.getElementById('cartTotal');

    function addToCart(name, price){
      cart.push({name, price});
      updateCart();
      alert(name + ' أضيف للسلة');
    }
    function updateCart(){
      if(cart.length===0){cartBox.style.display='none'; return}
      cartBox.style.display='block';
      const total = cart.reduce((s,p)=>s+p.price,0);
      cartTotalEl.textContent = total + ' ر.س';
    }
    function openCartOrder(){
      location.href = '#order';
      // transfer cart info to form details
      const det = document.getElementById('details');
      const list = cart.map(c=>c.name + ' ('+c.price+' ر.س)').join('\\n');
      det.value = (det.value?det.value+"\\n\\n":"") + "طلبات من السلة:\\n" + list;
    }

    // Toggle material (buttons)
    function toggleMaterial(name){
      if(selectedMaterials.has(name)){ selectedMaterials.delete(name); alert(name+' شالت من الطلب')}
      else{ selectedMaterials.add(name); alert(name+' اضيفت للطلب')}
      calcPrice();
    }

    // Prefill package
    function prefillPackage(pkg,price){
      document.getElementById('serviceType').value = 'اشتراك';
      document.getElementById('details').value = 'طلب باقة: '+pkg+' — السعر: '+price+' ر.س';
      document.getElementById('serviceDetails').style.display='block';
      calcPrice();
      location.href='#order';
    }

    // Service changed
    function serviceChanged(){
      const t = document.getElementById('serviceType').value;
      if(t){ document.getElementById('serviceDetails').style.display='block'; }
      else document.getElementById('serviceDetails').style.display='none';
      calcPrice();
    }

    // Pay method
    function payMethodChanged(){
      // nothing heavy here; form will carry selection
    }

    // Price calc: rough estimates
    function calcPrice(){
      const svc = document.getElementById('serviceType').value;
      const payMethod = document.getElementById('payMethod').value;
      let total = 0;
      // base by service
      if(svc==='واجب') total += 50;
      else if(svc==='مشروع') total += 120;
      else if(svc==='عرض') total += 60;
      else if(svc==='ملزمة') total += 35;
      else if(svc==='اشتراك') {
        // default per-material 180, if selectedMaterials size >1 apply 15% discount
        const count = Math.max(1, selectedMaterials.size || 1);
        let per = 180;
        if(count>=2) per = Math.round(per * 0.85); // 15% off
        total += per * count;
      }
      // add cart items
      total += cart.reduce((s,p)=>s+p.price,0);
      // show
      document.getElementById('calcTotal').textContent = total + ' ر.س';
      return total;
    }

    // On form submit -> prepare whatsapp message & open
    function handleSubmit(e){
      e.preventDefault();
      const name = document.getElementById('studentName').value.trim();
      const sid = document.getElementById('studentId').value.trim();
      const major = document.getElementById('major').value;
      const svc = document.getElementById('serviceType').value;
      const details = document.getElementById('details').value.trim();
      const pay = document.getElementById('payMethod').value;
      const total = calcPrice();

      // file name
      const fileInput = document.getElementById('fileUpload');
      const fileName = fileInput.files.length ? fileInput.files[0].name : 'لا يوجد';

      // materials
      const mats = Array.from(selectedMaterials).join(', ') || 'لا يوجد';

      // Build message
      let message = '🟢 طلب خدمة من منصة سند%0A';
      message += '*الاسم:* ' + encodeURIComponent(name) + '%0A';
      message += '*الرقم الجامعي:* ' + encodeURIComponent(sid) + '%0A';
      message += '*الكلية/التخصص:* ' + encodeURIComponent(major) + '%0A';
      message += '*نوع الخدمة:* ' + encodeURIComponent(svc) + '%0A';
      message += '*تفاصيل الطلب:* ' + encodeURIComponent(details || '-') + '%0A';
      message += '*الملفات المرفقة:* ' + encodeURIComponent(fileName) + '%0A';
      message += '*المواد المطلوبة:* ' + encodeURIComponent(mats) + '%0A';
      message += '*طريقة الدفع المفضلة:* ' + encodeURIComponent(pay) + '%0A';
      message += '*المبلغ التقريبي:* ' + encodeURIComponent(total + ' ر.س') + '%0A';
      message += '%0A' + encodeURIComponent('أرسلوا إيصال التحويل بعد الدفع حتى نفعل الطلب.');

      // open WhatsApp
      const wa = 'https://wa.me/966565885750?text=' + message;
      window.open(wa,'_blank');

      // optional: show toast or reset
      alert('تم تجهيز رسالة الطلب — افتح واتساب لإرسالها وتأكيد الطلب. بعد استلام الإيصال بنفعل الطلب.');
      return false;
    }

    // Reset
    function resetOrder(){
      document.getElementById('orderForm').reset();
      selectedMaterials = new Set();
      cart = [];
      updateCart();
      calcPrice();
      document.getElementById('serviceDetails').style.display='none';
    }

    // small interval calc
    setInterval(calcPrice,1000);

    // init
    updateCart();
    calcPrice();
  </script>
</body>
</html>
