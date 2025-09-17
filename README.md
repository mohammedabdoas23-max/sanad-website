<!doctype html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1"/>
<title>منصة سند | خدمات طلابية جامعة الملك سعود</title>
<meta name="description" content="منصة سند للخدمات الإلكترونية والتعليمية | حلول واجبات وكويزات، مشاريع وتقارير، عروض تقديمية، ملخصات ومراجعات – KSU">
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700;800&display=swap" rel="stylesheet">

<style>
:root{
  --ksu-deep:#0b2b5a;        /* أزرق كحلي */
  --ksu-blue:#114a9f;        /* أزرق */
  --ksu-sky:#2ea4ff;         /* أزرق سماوي */
  --gold:#d4af37;            /* ذهبي */
  --bg:#f7fafc;
  --card:#ffffff;
  --muted:#6b7280;
  --ring:#e0ecff;
  --ok:#16a34a;
  --warn:#eab308;
  --danger:#ef4444;
  --shadow:0 10px 26px rgba(11,43,90,.08);
  --radius:16px;
}
*{box-sizing:border-box}
html,body{margin:0;background:var(--bg);color:#0f172a;font-family:"Tajawal",system-ui,sans-serif}
a{color:var(--ksu-blue);text-decoration:none}
a:hover{opacity:.9}
.container{width:clamp(320px,92vw,1100px);margin-inline:auto;padding:18px}
.btn{
  display:inline-flex;align-items:center;gap:10px;cursor:pointer;
  padding:12px 18px;border-radius:12px;border:1px solid transparent;
  font-weight:700;transition:.15s background,.15s transform;
}
.btn:hover{transform:translateY(-1px)}
.btn.primary{background:var(--ksu-blue);color:#fff}
.btn.light{background:#fff;border-color:#eef2ff;color:var(--ksu-blue)}
.btn.gold{background:var(--gold);color:#111827}
.badge{background:#fff;color:var(--ksu-blue);border:1px solid #e5e7eb;border-radius:999px;padding:5px 10px;font-weight:700}
.card{
  background:var(--card);border:1px solid #eef2ff;border-radius:var(--radius);
  box-shadow:var(--shadow);padding:18px;
}
.grid{display:grid;gap:16px}
.grid.cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}
.grid.cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}
@media (max-width:900px){.grid.cols-3{grid-template-columns:repeat(2,1fr)}}
@media (max-width:640px){.grid.cols-3,.grid.cols-2{grid-template-columns:1fr}}
/* Header */
.topbar{
  background:linear-gradient(135deg,var(--ksu-deep),#0e3778 60%,#0b2b5a);
  color:#fff;border-bottom:3px solid var(--gold);
}
.nav{display:flex;align-items:center;justify-content:space-between;gap:14px}
.brand{display:flex;align-items:center;gap:12px}
.logo{
  width:42px;height:42px;border-radius:10px;
  background:
    radial-gradient(12px 12px at 65% 65%,#fff0 70%,#fff 72%),
    conic-gradient(from 200deg at 45% 45%,#fff0 0 40%,#fff 0 48%,#fff0 0 100%),
    linear-gradient(180deg,#1a56b5,#0e3f8f);
  outline:3px solid #fff2;box-shadow:0 2px 0 0 #0003 inset;
}
.brand h1{font-size:20px;margin:0;font-weight:800;letter-spacing:.2px}
.menu{display:flex;gap:10px;flex-wrap:wrap}
.menu a{color:#e6efff;background:#ffffff1a;border:1px solid #ffffff33;padding:8px 12px;border-radius:10px}
.menu a:hover{background:#ffffff26}
.hero{
  background:
    radial-gradient(600px 220px at 85% -40%,#2ea4ff20 30%,#ffffff00 70%),
    radial-gradient(600px 220px at -10% 130%,#d4af3718 30%,#ffffff00 70%);
  color:#fff;padding:36px 0 30px
}
.hero h2{margin:8px 0 10px;font-size:30px}
.hero p{color:#e3eeff;margin:0 0 16px}
/* tabs */
.tabs{display:flex;gap:10px;flex-wrap:wrap;margin:6px 0 14px}
.tab{padding:8px 12px;border-radius:10px;border:1px solid #e5e7eb;cursor:pointer;background:#fff;font-weight:700}
.tab.active{background:var(--ksu-blue);color:#fff;border-color:transparent}
/* forms */
.form{display:grid;gap:12px}
.input,.select,.textarea{
  width:100%;padding:12px 14px;border-radius:12px;border:1px solid #e5e7eb;background:#fff;
}
.textarea{min-height:110px}
.small{font-size:13px;color:var(--muted)}
.kit{display:flex;gap:10px;flex-wrap:wrap}
.kit .chip{background:#f3f6ff;border:1px dashed #d7e6ff;color:#0b2b5a;padding:8px 10px;border-radius:10px}
.price{font-weight:800;color:var(--ksu-blue)}
/* accordion */
.acc{display:grid;gap:10px}
.acc details{border:1px solid #e5e7eb;border-radius:12px;background:#fff}
.acc summary{list-style:none;cursor:pointer;padding:14px 16px;font-weight:800;color:#0f172a}
.acc summary::-webkit-details-marker{display:none}
.acc .content{padding:0 16px 16px}
.hr{height:1px;background:#eef2ff;margin:18px 0}
/* footer */
.footer{background:var(--ksu-deep);color:#dbe8ff;padding:32px 0;margin-top:26px;border-top:3px solid var(--gold)}
.footer a{color:#dbe8ff}
.center{text-align:center}
.hidden{display:none}
</style>
</head>

<body>

<!-- ===== Header / Hero ===== -->
<header class="topbar">
  <div class="container nav">
    <div class="brand">
      <div class="logo" aria-hidden="true"></div>
      <h1>منصة سند <span class="badge">KSU</span></h1>
    </div>
    <nav class="menu">
      <a href="#services">الخدمات</a>
      <a href="#first-year">المواد المشتركة</a>
      <a href="#bundles">الباقات</a>
      <a href="#experts">للمختصين</a>
      <a href="#join">انضمام للفريق</a>
      <a href="#contact">تواصل</a>
    </nav>
  </div>

  <div class="container hero">
    <h2>خدمات طلابية متكاملة — جامعة الملك سعود</h2>
    <p>حلول واجبات وكويزات، تنفيذ مشاريع وتقارير، عروض تقديمية، ملخصات ومراجعات — شغل نظيف، التزام بالمواعيد، ومتابعة خاصة.</p>
    <div class="kit">
      <a class="btn primary" href="#first-year">ابدأ من المواد المشتركة</a>
      <a class="btn light" href="https://t.me/iTx7llxb_15" target="_blank" rel="noopener">تواصل تيليجرام</a>
      <a class="btn gold" href="https://wa.me/966565885750" target="_blank" rel="noopener">واتساب مباشر</a>
    </div>
  </div>
</header>

<main class="container">

  <!-- ===== quick services ===== -->
  <section id="services" class="grid cols-3" aria-label="الخدمات السريعة">
    <div class="card">
      <h3>حلول سريعة</h3>
      <p class="small">كويزات وواجبات مع ضمان الدقة والتسليم ضمن الوقت.</p>
      <div class="kit"><span class="chip">نهج/فجب/تقن</span><span class="chip">رياضيات/إحصاء</span></div>
    </div>
    <div class="card">
      <h3>مشاريع وتقارير</h3>
      <p class="small">تنفيذ كامل مع ترتيب المراجع والتنسيق حسب دليل المقرر.</p>
      <div class="kit"><span class="chip">APA7 / IEEE</span><span class="chip">LaTeX / Word</span></div>
    </div>
    <div class="card">
      <h3>عروض تقديمية وملخصات</h3>
      <p class="small">تصاميم احترافية + ملخصات مفهرسة وتجميعات قبل الاختبارات.</p>
      <div class="kit"><span class="chip">بوربوينت</span><span class="chip">PDF</span></div>
    </div>
  </section>

  <div class="hr"></div>

  <!-- ===== First Year Shared ===== -->
  <section id="first-year">
    <h2>السنة الأولى المشتركة – المواد الأساسية</h2>
    <p class="small">المسارات: علمي • صحي • إداري • إنساني — وبعض المواد مشتركة بين الجميع.</p>

    <div class="tabs" id="fyTabs">
      <button class="tab active" data-subject="نهج 101">نهج 101</button>
      <button class="tab" data-subject="فجب 101">فجب 101</button>
      <button class="tab" data-subject="تقن 101">تقن 101</button>
      <button class="tab" data-subject="إنجل 101">إنجل 101</button>
      <button class="tab" data-subject="ريد 101">ريد 101</button>
      <button class="tab" data-subject="عرب 101">عرب 101</button>
      <button class="tab" data-subject="إحص 101">إحص 101</button>
    </div>

    <!-- tasks / accordion -->
    <div class="acc">
      <details open>
        <summary>قوالب التكاليف الأكثر طلبًا</summary>
        <div class="content grid cols-2">
          <div class="card">
            <h3>تكليف واحد</h3>
            <p class="small">اختَر نوع التكليف وارسِل تفاصيل الدكتور. <span class="price">50 ر.س</span></p>
            <div class="form">
              <select id="taskType" class="select">
                <option>توثيق المراجع APA7</option>
                <option>التكليف البحثي (الوصول للمعلومات)</option>
                <option>عرض تقديمي</option>
                <option>خريطة ذهنية</option>
                <option>حل واجب</option>
              </select>
              <input class="input" id="stdName" placeholder="اسمك (اختياري)"/>
              <div class="grid cols-2">
                <input class="input" id="stdId" placeholder="الرقم الجامعي (اختياري)"/>
                <input class="input" id="sectionNo" placeholder="رقم الشعبة (اختياري)"/>
              </div>
              <textarea class="textarea" id="taskNotes" placeholder="اكتب المتطلبات أو نقاط الدكتور"></textarea>
              <p class="small">عندك ملف/صورة للتكليف؟ ارفعه مع الرسالة بعد ما تفتح واتساب/تيليجرام.</p>
              <div class="kit">
                <button class="btn primary" onclick="sendTask('whatsapp')">إرسال واتساب</button>
                <button class="btn light"   onclick="sendTask('telegram')">إرسال تيليجرام</button>
              </div>
            </div>
          </div>

          <div class="card">
            <h3>باقة 3 تكاليف</h3>
            <p class="small">مثال: عرض + خريطة + بحث. <span class="price">100 ر.س</span></p>
            <div class="form">
              <input class="input" id="bundleSubject" placeholder="المادة (مثال: نهج 101)"/>
              <textarea class="textarea" id="bundleList" placeholder="اذكر التكاليف الثلاثة المطلوبة"></textarea>
              <div class="kit">
                <button class="btn primary" onclick="sendBundle('whatsapp')">طلب الباقة واتساب</button>
                <button class="btn light"   onclick="sendBundle('telegram')">طلب الباقة تيليجرام</button>
              </div>
            </div>
          </div>
        </div>
      </details>

      <details>
        <summary>اشتراك شامل للمادة (ميد + فاينل)</summary>
        <div class="content card">
          <p>الاشتراك يشمل متابعة الأعمال الفصلية + حل الواجبات والكويزات + ملخصات ومراجعات وتجميعات قبل الاختبار.</p>
          <div class="form">
            <label>اختر المواد وعددها (يحسب الخصم تلقائي):</label>
            <div class="grid cols-3">
              <label><input type="checkbox" class="subCheck" value="نهج 101"> نهج 101</label>
              <label><input type="checkbox" class="subCheck" value="فجب 101"> فجب 101</label>
              <label><input type="checkbox" class="subCheck" value="تقن 101"> تقن 101</label>
              <label><input type="checkbox" class="subCheck" value="إنجل 101"> إنجل 101</label>
              <label><input type="checkbox" class="subCheck" value="ريد 101"> ريد 101</label>
              <label><input type="checkbox" class="subCheck" value="عرب 101"> عرب 101</label>
              <label><input type="checkbox" class="subCheck" value="إحص 101"> إحص 101</label>
            </div>
            <div class="card" style="background:#f8fbff;border-color:#e0ecff">
              <div id="subCalc" class="small">السعر الأساسي: 180 ر.س لكل مادة. إذا اخترت مادتين أو أكثر: خصم 15% → 153 ر.س للمادة.</div>
              <div style="display:flex;gap:10px;align-items:center;margin-top:8px">
                <strong>الإجمالي:</strong> <span id="totalPrice" class="price">0 ر.س</span>
              </div>
            </div>
            <input class="input" id="subscriberName" placeholder="اسمك" />
            <textarea class="textarea" id="subscriberNotes" placeholder="اذكر ملاحظاتك (أوقات الكويزات إن وجدت، ظروف المادة، إلخ)"></textarea>
            <div class="kit">
              <button class="btn primary" onclick="sendSubscription('whatsapp')">اشتراك – واتساب</button>
              <button class="btn light"   onclick="sendSubscription('telegram')">اشتراك – تيليجرام</button>
            </div>
          </div>
        </div>
      </details>
    </div>
  </section>

  <div class="hr"></div>

  <!-- ===== Bundles (generic) ===== -->
  <section id="bundles">
    <h2>باقات وتخصصات</h2>
    <p class="small">نغطي جميع المواد والتخصصات: علمي، صحي، إداري، إنساني — + علوم أساسية (فيزياء/كيمياء/أحياء/رياضيات/إحصاء).</p>
    <div class="grid cols-3">
      <div class="card">
        <h3>🧪 العلوم</h3>
        <p class="small">فيزياء/كيمياء/أحياء عامة ومخبرية – تقارير، بحوث، تجارب، عروض.</p>
        <button class="btn primary" onclick="openGeneric('العلوم')">اطلب خدمة</button>
      </div>
      <div class="card">
        <h3>💼 الإداري</h3>
        <p class="small">اقتصاد، محاسبة، نظم معلومات، إدارة – كويزات، مشاريع حالة، عروض.</p>
        <button class="btn primary" onclick="openGeneric('الإداري')">اطلب خدمة</button>
      </div>
      <div class="card">
        <h3>🧑‍⚕️ الصحي</h3>
        <p class="small">أحياء دقيقة، تغذية، تمريض، صحة عامة – تقارير مختبر ومراجعات.</p>
        <button class="btn primary" onclick="openGeneric('الصحي')">اطلب خدمة</button>
      </div>
      <div class="card">
        <h3>📚 الإنساني</h3>
        <p class="small">لغة عربية، تربية، تاريخ، إعلام – بحوث وعروض ومهام مقررات.</p>
        <button class="btn primary" onclick="openGeneric('الإنساني')">اطلب خدمة</button>
      </div>
      <div class="card">
        <h3>💻 الحاسب والتقنية</h3>
        <p class="small">برمجة، قواعد بيانات، شبكات – مشاريع، تقارير تقنية، سحب أكواد.</p>
        <button class="btn primary" onclick="openGeneric('الحاسب والتقنية')">اطلب خدمة</button>
      </div>
      <div class="card">
        <h3>🧮 رياضيات وإحصاء</h3>
        <p class="small">حل مسائل، نمذجة، واجبات، كويزات – شرح مبسّط وخطوات الحل.</p>
        <button class="btn primary" onclick="openGeneric('الرياضيات والإحصاء')">اطلب خدمة</button>
      </div>
    </div>
  </section>

  <div class="hr"></div>

  <!-- ===== Experts & Join ===== -->
  <section id="experts" class="grid cols-2">
    <div class="card">
      <h3>للمختصين ومالكي المحتوى</h3>
      <p class="small">عندك ملخصات/ملازم/قناة شرح وتبغى تعرضها داخل منصة سند؟ عَبّ النموذج وننسّق معك (نسبة عادلة أو اشتراك).</p>
      <div class="form">
        <input id="vendorName" class="input" placeholder="اسمك/اسم الجهة"/>
        <input id="vendorLink" class="input" placeholder="رابط عينة (قناة/ملف)"/>
        <textarea id="vendorNotes" class="textarea" placeholder="نبذة عن المحتوى، السعر المقترح، وآلية التسليم"></textarea>
        <div class="kit">
          <button class="btn primary" onclick="sendVendor('whatsapp')">إرسال – واتساب</button>
          <button class="btn light"   onclick="sendVendor('telegram')">إرسال – تيليجرام</button>
        </div>
      </div>
    </div>

    <div id="join" class="card">
      <h3>انضم لفريق منصة سند</h3>
      <p class="small">طالب/خريج وتقدر تشرح مقرر أو تصمم ملخصات؟ قدّم وخلنا نرتّب لك دخل حلو (نسبة من الخدمة أو باقة شهرية).</p>
      <div class="form">
        <input id="coachName" class="input" placeholder="اسمك الكامل"/>
        <input id="coachMajor" class="input" placeholder="التخصص/الكلية"/>
        <input id="coachCourses" class="input" placeholder="المقررات اللي تقدر تشرحها"/>
        <textarea id="coachNotes" class="textarea" placeholder="خبرتك، مستواك، فكرة المحتوى اللي تبغى تقدّمه"></textarea>
        <p class="small">عندك شرح تجريبي؟ ارفعه وأرسل الرابط هنا، وبعد الإرسال أرفق المقطع في التيليجرام.</p>
        <div class="kit">
          <button class="btn primary" onclick="sendCoach('whatsapp')">تقديم – واتساب</button>
          <button class="btn light"   onclick="sendCoach('telegram')">تقديم – تيليجرام</button>
        </div>
      </div>
    </div>
  </section>

  <div class="hr"></div>

  <!-- ===== Payment & Contact ===== -->
  <section id="contact" class="grid cols-2">
    <div class="card">
      <h3>🏦 بيانات التحويل اليدوي (STC Pay / بنك محلي)</h3>
      <ul class="small" style="margin:0;padding-inline-start:18px;line-height:1.9">
        <li><strong>البنك:</strong> البنك العربي الوطني السعودي (anb)</li>
        <li><strong>اسم المستفيد:</strong> عزام عبدالله عبدالعزيز ناجي</li>
        <li><strong>رقم الحساب:</strong> <code>942000177167245</code></li>
        <li><strong>الآيبان:</strong> <code>SA0530100942000177167245</code></li>
      </ul>
      <p class="small">بعد التحويل، أرسل إيصال الدفع على واتساب أو تيليجرام لتأكيد الطلب – يتم التأكيد بسرعة ويوصلك المحتوى تلقائيًا.</p>
      <div class="kit">
        <a class="btn light"  href="https://wa.me/966565885750?text=تم%20التحويل%20وهذا%20الإيصال" target="_blank" rel="noopener">إرفاق الإيصال – واتساب</a>
        <a class="btn primary" href="https://t.me/iTx7llxb_15" target="_blank" rel="noopener">مراسلة تيليجرام</a>
      </div>
    </div>

    <div class="card center">
      <h3>قنوات المنصة</h3>
      <p class="small">للمتجر، التحديثات، ونماذج الأعمال.</p>
      <div class="kit" style="justify-content:center">
        <a class="btn primary" href="https://t.me/Helping_KSU" target="_blank" rel="noopener">📣 قناة المتجر</a>
        <a class="btn light"   href="https://t.me/student_services24" target="_blank" rel="noopener">📢 قناة الأعمال</a>
      </div>
    </div>
  </section>

</main>

<!-- ===== Footer ===== -->
<footer class="footer">
  <div class="container center">
    <div style="margin-bottom:8px">
      <strong>© 2025 منصة سند للخدمات الإلكترونية والتعليمية.</strong> جميع الحقوق محفوظة.
    </div>
    <div class="small">
      <a href="#bundles">قائمة الخدمات</a> •
      <a href="#first-year">المواد المشتركة</a> •
      <a href="#contact">اطلب خدمة</a>
    </div>
  </div>
</footer>

<script>
/* تبويب المادة الحالي (شكلي فقط) */
document.querySelectorAll('#fyTabs .tab').forEach(btn=>{
  btn.addEventListener('click',()=>{
    document.querySelectorAll('#fyTabs .tab').forEach(b=>b.classList.remove('active'));
    btn.classList.add('active');
  });
});

/* بناء نص واتساب/تيليجرام */
const WAPP = "https://wa.me/966565885750?text=";
const TG   = "https://t.me/iTx7llxb_15";

function openLink(type, message){
  const encoded = encodeURIComponent(message);
  if(type==='whatsapp') window.open(WAPP+encoded,'_blank');
  else window.open(TG,'_blank');
}

/* طلب تكليف واحد */
function sendTask(type){
  const subject = document.querySelector('#fyTabs .tab.active').dataset.subject;
  const task    = document.getElementById('taskType').value;
  const name    = document.getElementById('stdName').value.trim();
  const id      = document.getElementById('stdId').value.trim();
  const sec     = document.getElementById('sectionNo').value.trim();
  const notes   = document.getElementById('taskNotes').value.trim();

  let msg = `السلام عليكم 👋\nأبغى أطلب تكليف لمادة (${subject}).\n\nالنوع: ${task}\nالسعر: 50 ر.س ✅\n\nالبيانات:\n`;
  if(name) msg += `- الاسم: ${name}\n`;
  if(id)   msg += `- الرقم الجامعي: ${id}\n`;
  if(sec)  msg += `- رقم الشعبة: ${sec}\n`;
  if(notes)msg += `\nملاحظات/متطلبات الدكتور:\n${notes}\n`;
  msg += `\nأرفق الإيصال بعد التأكيد، وشكرًا.`;

  openLink(type,msg);
}

/* باقة 3 تكاليف */
function sendBundle(type){
  const subject = document.getElementById('bundleSubject').value || document.querySelector('#fyTabs .tab.active').dataset.subject;
  const list    = document.getElementById('bundleList').value.trim();
  let msg = `تحية طيبة 🌟\nأرغب بباقة 3 تكاليف لمادة (${subject}).\nالسعر الإجمالي: 100 ر.س ✅\n\nالتكاليف المطلوبة:\n${list || '- سيتم تحديدها معاكم'}\n\nأكّدوا التوفر والمواعيد.`;
  openLink(type,msg);
}

/* اشتراك شامل – حساب الخصم */
const BASE = 180, DISCOUNT = 0.15;
function calcTotal(){
  const checks=[...document.querySelectorAll('.subCheck')].filter(c=>c.checked).map(c=>c.value);
  let per = (checks.length >= 2) ? Math.round(BASE*(1-DISCOUNT)) : BASE;
  let total = checks.length * per;
  document.getElementById('totalPrice').textContent = `${total} ر.س`;
  return {checks, per, total};
}
document.querySelectorAll('.subCheck').forEach(c=>c.addEventListener('change',calcTotal));

function sendSubscription(type){
  const {checks, per, total} = calcTotal();
  const name = document.getElementById('subscriberName').value.trim();
  const notes= document.getElementById('subscriberNotes').value.trim();
  if(checks.length===0){ alert('اختَر مادة أو أكثر للاشتراك.'); return; }
  let msg = `السلام عليكم 👋\nأرغب باشتراك شامل للمادة/المواد التالية:\n- ${checks.join('\n- ')}\n`;
  msg += (checks.length>=2)?`\n(تطبيق خصم 15% – ${per} ر.س للمادة)`:`\nالسعر للمادة: ${per} ر.س`;
  msg += `\nالإجمالي: ${total} ر.س ✅\n`;
  if(name) msg += `\nالاسم: ${name}`;
  if(notes)msg += `\nملاحظات:\n${notes}`;
  openLink(type,msg);
}

/* طلب عام للتخصصات */
function openGeneric(track){
  const subject = prompt(`اكتب اسم المادة داخل مسار: ${track} (مثال: كيمياء عامة 101)`) || `${track} - مادة غير محددة`;
  const service = prompt("اذكر الخدمة المطلوبة (كويز/واجب/مشروع/عرض/ملخص...)") || "خدمة غير محددة";
  const date    = prompt("موعد التسليم/الاختبار (اختياري)") || "";
  let msg = `السلام عليكم 👋\nطلب خدمة لمسار: ${track}\nالمادة: ${subject}\nالخدمة: ${service}`;
  if(date) msg += `\nالموعد: ${date}`;
  msg += `\n\nأرسلوا لي السعر والتفاصيل وطريقة الدفع.`;
  openLink('whatsapp',msg);
}

/* للمختصين */
function sendVendor(type){
  const n = document.getElementById('vendorName').value.trim();
  const l = document.getElementById('vendorLink').value.trim();
  const t = document.getElementById('vendorNotes').value.trim();
  let msg = `مرحبًا، لدي محتوى تعليمي أرغب بعرضه في منصة سند.\nالاسم/الجهة: ${n||'-'}\nرابط عينة: ${l||'-'}\nتفاصيل وسعر مقترح:\n${t||'-'}`;
  openLink(type,msg);
}

/* انضمام للفريق */
function sendCoach(type){
  const n = document.getElementById('coachName').value.trim();
  const m = document.getElementById('coachMajor').value.trim();
  const c = document.getElementById('coachCourses').value.trim();
  const t = document.getElementById('coachNotes').value.trim();
  let msg = `السلام عليكم، أرغب بالانضمام لفريق منصة سند.\nالاسم: ${n||'-'}\nالتخصص/الكلية: ${m||'-'}\nالمقررات القابلة للشرح: ${c||'-'}\nملاحظات/خبرة:\n${t||'-'}\n(سأرسل عينة الشرح في التيليجرام).`;
  openLink(type,msg);
}

/* تحديث الإجمالي عند الفتح */
calcTotal();
</script>
</body>
</html>
