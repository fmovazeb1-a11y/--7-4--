# --7-4--
<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AMIR SG | تحقیقات علوم هفتم</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Vazirmatn:wght@400;500;600;700;800;900&display=swap');

:root {
  --blue: #268cff;
  --cyan: #16c9d8;
  --purple: #9b70f5;
  --orange: #ffad52;
  --pink: #ff79b9;
  --dark: #14223c;
}

* {
  box-sizing: border-box;
  scroll-behavior: smooth;
}

body {
  margin: 0;
  font-family: Vazirmatn, Tahoma, sans-serif;
  color: #172b49;
  background:
    radial-gradient(circle at 10% 10%, #a8e8ff 0, transparent 30%),
    radial-gradient(circle at 90% 20%, #ffd2e9 0, transparent 28%),
    radial-gradient(circle at 15% 85%, #d6c4ff 0, transparent 32%),
    radial-gradient(circle at 90% 90%, #ffe1a8 0, transparent 30%),
    linear-gradient(135deg, #e6faff, #f5eaff, #fff3e3);
  min-height: 100vh;
  overflow-x: hidden;
}

/* واترمارک تکرارشونده */
body::before {
  content:
    "امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب • امیرحسین مواظب";
  position: fixed;
  inset: -80px;
  z-index: -1;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  line-height: 4;
  letter-spacing: 3px;
  word-spacing: 18px;
  font-size: 15px;
  font-weight: 900;
  color: rgba(50, 111, 185, .13);
  transform: rotate(-19deg) scale(1.3);
  pointer-events: none;
}

header {
  background: rgba(255,255,255,.76);
  backdrop-filter: blur(15px);
  border-bottom: 1px solid rgba(255,255,255,.9);
  padding: 17px 6%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: 14px;
  position: sticky;
  top: 0;
  z-index: 10;
  box-shadow: 0 5px 25px rgba(45,90,150,.08);
}

.logo {
  font-size: 25px;
  font-weight: 900;
  color: #2468c9;
  letter-spacing: 2px;
}

.logo span {
  color: #14b9bd;
}

nav {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

nav a {
  text-decoration: none;
  color: #314767;
  font-size: 14px;
  font-weight: 700;
  padding: 9px 13px;
  border-radius: 12px;
  transition: .2s;
}

nav a:hover {
  background: #dcecff;
  color: #1268d2;
}

.hero {
  text-align: center;
  padding: 75px 20px 55px;
}

.tag {
  display: inline-block;
  background: white;
  color: #2476d8;
  padding: 9px 18px;
  border-radius: 50px;
  font-size: 12px;
  font-weight: 800;
  box-shadow: 0 5px 20px rgba(50,100,160,.1);
}

.hero h1 {
  font-size: clamp(32px, 6vw, 58px);
  margin: 22px 0 12px;
  color: #1d3c67;
  font-weight: 900;
}

.hero h1 span {
  background: linear-gradient(90deg,#168bdf,#8d69ec,#ed75ae);
  -webkit-background-clip: text;
  color: transparent;
}

.hero p {
  color: #536b89;
  line-height: 2.1;
  max-width: 700px;
  margin: auto;
}

.container {
  width: min(1050px, 92%);
  margin: auto;
}

.section-title {
  font-size: 26px;
  color: #23436d;
  margin: 35px 0 20px;
}

.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit,minmax(230px,1fr));
  gap: 18px;
}

.card {
  background: rgba(255,255,255,.86);
  border: 1px solid white;
  padding: 23px;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(48,91,150,.09);
  transition: .25s;
}

.card:hover {
  transform: translateY(-6px);
}

.card h3 {
  margin-top: 0;
  color: #2676d5;
}

.card p {
  color: #647994;
  line-height: 1.9;
}

.lesson {
  background: rgba(255,255,255,.9);
  border: 1px solid white;
  border-radius: 22px;
  padding: 25px;
  margin: 28px 0;
  box-shadow: 0 12px 35px rgba(45,83,135,.1);
  scroll-margin-top: 100px;
}

.lesson h2 {
  color: #2474cf;
  font-size: 23px;
  border-right: 5px solid #20c4ca;
  padding-right: 13px;
}

.lesson h3 {
  color: #7959cb;
  margin-top: 27px;
}

.lesson p, .lesson li {
  line-height: 2.2;
  color: #425a79;
}

.lesson ul {
  padding-right: 25px;
}

.answer {
  background: #eef7ff;
  border-right: 4px solid #3299e8;
  padding: 15px 17px;
  margin: 13px 0;
  border-radius: 12px;
  line-height: 2.1;
  color: #354f70;
}

.green {
  background: #e9faf4;
  border-color: #27b98b;
}

.purple {
  background: #f2edff;
  border-color: #9875e8;
}

.orange {
  background: #fff5e8;
  border-color: #f3a94d;
}

.pink {
  background: #fff0f7;
  border-color: #eb80b3;
}

table {
  width: 100%;
  border-collapse: collapse;
  overflow: hidden;
  border-radius: 12px;
  margin: 15px 0;
  background: white;
}

th, td {
  padding: 13px;
  border: 1px solid #dce9f5;
  text-align: right;
  line-height: 1.8;
}

th {
  background: #dceeff;
  color: #245c9e;
}

button {
  font-family: inherit;
  border: none;
  background: linear-gradient(110deg,#2588ed,#16beca);
  color: white;
  padding: 12px 19px;
  border-radius: 12px;
  cursor: pointer;
  font-weight: 800;
  transition: .2s;
}

button:hover {
  transform: translateY(-2px);
  filter: brightness(1.06);
}

footer {
  text-align: center;
  margin-top: 60px;
  padding: 35px 15px;
  background: rgba(255,255,255,.8);
  border-top: 1px solid white;
  color: #607793;
  line-height: 2.3;
}

footer strong {
  color: #2476d5;
}

@media(max-width:600px) {
  header {
    justify-content: center;
  }
  nav {
    justify-content: center;
  }
  .lesson {
    padding: 18px;
  }
  th,td {
    padding: 9px;
    font-size: 13px;
  }
}
</style>
</head>

<body>

<header>
  <div class="logo">AMIR <span>SG</span></div>
  <nav>
    <a href="#home">خانه</a>
    <a href="#research1">تحقیق اول</a>
    <a href="#research2">تحقیق دوم</a>
    <a href="#result">نتیجه‌گیری</a>
  </nav>
</header>

<section class="hero" id="home">
  <div class="tag">SCIENCE RESEARCH • GRADE 7</div>
  <h1>تحقیقات <span>علوم تجربی</span></h1>
  <p>
    بررسی دو موضوع مهم درباره چرخه آب، بارورسازی ابرها
    و منابع تأمین آب استان تهران
  </p>
  <p>تهیه و تنظیم: امیرحسین مواظب</p>
  <br>
  <a href="#research1"><button>شروع مطالعه</button></a>
</section>

<main class="container">

<section>
  <h2 class="section-title">موضوعات تحقیق</h2>
  <div class="cards">
    <div class="card">
      <h3>تحقیق اول: بارورسازی ابرها</h3>
      <p>بررسی چگونگی بارور کردن ابرها، مواد مورد استفاده، روش‌ها و فواید آن.</p>
      <a href="#research1"><button>مطالعه تحقیق</button></a>
    </div>

    <div class="card">
      <h3>تحقیق دوم: منابع آب تهران</h3>
      <p>بررسی آب‌های سطحی و زیرزمینی و منابع تأمین آب استان تهران.</p>
      <a href="#research2"><button>مطالعه تحقیق</button></a>
    </div>
  </div>
</section>

<!-- تحقیق اول -->

<section class="lesson" id="research1">
  <h2>تحقیق اول: بارور کردن ابرها و تشکیل باران مصنوعی</h2>

  <h3>۱. بارورسازی ابرها چیست؟</h3>
  <p>
    بارورسازی ابرها یا باران‌زایی مصنوعی، روشی علمی برای
    تأثیر گذاشتن بر فرایند طبیعی تشکیل باران یا برف است.
    در این روش، ذرات خاصی به بعضی ابرهای مناسب وارد می‌شوند
    تا شرایط رشد قطرات آب یا بلورهای یخ بهتر فراهم شود.
  </p>

  <div class="answer purple">
    <b>نکته مهم:</b>
    باران مصنوعی به معنی ساختن ابر یا تولید آب از هیچ نیست.
    این روش فقط تلاش می‌کند بارش یک ابر مناسب را تقویت کند.
  </div>

  <h3>۲. بارورسازی ابرها چگونه انجام می‌شود؟</h3>
  <p>
    درون ابرها قطرات بسیار ریز آب و گاهی بلورهای یخ وجود دارند.
    در عملیات بارورسازی، ذراتی مانند یدید نقره یا بعضی نمک‌ها
    وارد ابر می‌شوند. این ذرات در شرایط مناسب به تشکیل بلورهای
    یخ یا رشد قطرات آب کمک می‌کنند. با بزرگ‌تر و سنگین‌تر شدن
    این ذرات، ممکن است باران یا برف تشکیل شود.
  </p>

  <h3>۳. مواد مورد استفاده</h3>
  <div class="answer">
    <b>یدید نقره:</b>
    ماده‌ای که ساختار آن می‌تواند به تشکیل بلورهای یخ در
    بعضی ابرهای سرد کمک کند.
  </div>
  <div class="answer">
    <b>برخی نمک‌ها:</b>
    موادی که در بعضی ابرهای گرم می‌توانند به رشد قطرات آب کمک کنند.
  </div>

  <h3>۴. روش‌های بارورسازی</h3>
  <div class="answer">
    <b>روش هوایی:</b>
    با استفاده از هواپیما، مواد بارورساز در شرایط مناسب وارد ابرها می‌شوند.
  </div>
  <div class="answer">
    <b>روش زمینی:</b>
    از تجهیزات ویژه زمینی برای پخش ذرات در جریان هوا استفاده می‌شود
    تا این ذرات به ابرهای مناسب برسند.
  </div>

  <h3>۵. آیا هر ابری را می‌توان بارور کرد؟</h3>
  <p>
    خیر. برای بارورسازی، وجود ابر مناسب و شرایط جوی مشخص ضروری است.
    اگر رطوبت کافی یا شرایط مناسب وجود نداشته باشد، این روش
    نمی‌تواند از آسمان صاف باران ایجاد کند.
  </p>

  <h3>۶. فواید بارورسازی ابرها</h3>
  <ul>
    <li>امکان افزایش بارش در بعضی شرایط جوی.</li>
    <li>کمک احتمالی به افزایش ذخایر آب سطحی و زیرزمینی.</li>
    <li>امکان افزایش بارش برف در برخی مناطق کوهستانی.</li>
    <li>استفاده به‌عنوان یکی از روش‌های کمکی مدیریت منابع آب.</li>
  </ul>

  <h3>۷. محدودیت‌ها و مشکلات</h3>
  <ul>
    <li>نتیجه بارورسازی قطعی نیست.</li>
    <li>به شرایط طبیعی ابرها وابستگی زیادی دارد.</li>
    <li>اجرای آن نیازمند تجهیزات و دانش تخصصی است.</li>
    <li>اثر مواد استفاده‌شده بر محیط زیست باید بررسی شود.</li>
  </ul>

  <h3>۸. تفاوت باران طبیعی و باران حاصل از بارورسازی</h3>
  <table>
    <tr>
      <th>باران طبیعی</th>
      <th>بارش پس از بارورسازی</th>
    </tr>
    <tr>
      <td>بدون دخالت عمدی انسان شکل می‌گیرد.</td>
      <td>انسان تلاش می‌کند فرایند بارش را تقویت کند.</td>
    </tr>
    <tr>
      <td>به شرایط طبیعی جو وابسته است.</td>
      <td>به شرایط طبیعی و عملیات بارورسازی وابسته است.</td>
    </tr>
  </table>

  <div class="answer green">
    <b>نتیجه تحقیق اول:</b>
    بارورسازی ابرها یک روش علمی برای افزایش احتمالی بارش
    در شرایط مناسب است. این روش می‌تواند به مدیریت منابع آب کمک کند،
    اما راه‌حل قطعی خشکسالی نیست و جایگزین صرفه‌جویی در مصرف آب نمی‌شود.
  </div>
</section>

<!-- تحقیق دوم -->

<section class="lesson" id="research2">
  <h2>تحقیق دوم: منابع تأمین آب استان تهران</h2>

  <h3>سؤال کتاب:</h3>
  <div class="answer orange">
    در استان محل سکونت شما برای تأمین آب مصرفی بیشتر از آب‌های
    زیرزمینی استفاده می‌شود یا آب‌های سطحی؟ دلیل خود را در کلاس ارائه کنید.
  </div>

  <h3>۱. پاسخ کلی درباره استان تهران</h3>
  <p>
    در استان تهران از هر دو منبع آب‌های سطحی و زیرزمینی برای
    تأمین آب استفاده می‌شود. در تأمین آب آشامیدنی شهر تهران،
    آب‌های سطحی معمولاً سهم بیشتری دارند؛ اما آب‌های زیرزمینی
    نیز بخش مهمی از نیاز آبی را تأمین می‌کنند.
    مقدار استفاده از هر منبع با توجه به بارندگی، ذخیره سدها،
    خشکسالی و میزان مصرف تغییر می‌کند.
  </p>

  <div class="answer purple">
    <b>توجه:</b>
    سهم منابع آب برای تمام شهرستان‌های استان تهران یکسان نیست.
    همچنین سهم آب آشامیدنی شهر تهران را نباید با کل مصرف آب
    استان، شامل کشاورزی و صنعت، یکی دانست.
  </div>

  <h3>۲. منابع آب سطحی تهران</h3>
  <p>
    آب‌های سطحی شامل رودخانه‌ها و آب ذخیره‌شده پشت سدها هستند.
    مهم‌ترین سدهایی که در تأمین آب تهران نقش دارند عبارت‌اند از:
  </p>

  <ul>
    <li>سد امیرکبیر یا کرج</li>
    <li>سد طالقان</li>
    <li>سد لار</li>
    <li>سد لتیان</li>
    <li>سد ماملو</li>
  </ul>

  <p>
    آب این منابع پس از انتقال به تصفیه‌خانه‌ها و انجام مراحل
    تصفیه و کنترل کیفیت، وارد شبکه توزیع می‌شود.
  </p>

  <h3>۳. منابع آب زیرزمینی تهران</h3>
  <p>
    بخشی از آب باران و برف در زمین نفوذ می‌کند و در فضاهای خالی
    خاک و شکاف سنگ‌ها جمع می‌شود. این آب‌ها منابع زیرزمینی را
    تشکیل می‌دهند. برای استفاده از آن‌ها، آب از طریق چاه‌ها
    برداشت می‌شود.
  </p>

  <h3>۴. چرا تهران به هر دو منبع نیاز دارد؟</h3>
  <ul>
    <li>جمعیت زیاد تهران باعث افزایش نیاز به آب شده است.</li>
    <li>میزان بارندگی در فصل‌های مختلف یکسان نیست.</li>
    <li>در زمان خشکسالی، ذخیره سدها کاهش پیدا می‌کند.</li>
    <li>آب‌های زیرزمینی می‌توانند بخشی از کمبود منابع سطحی را جبران کنند.</li>
    <li>تأمین آب پایدار به استفاده و مدیریت درست هر دو منبع نیاز دارد.</li>
  </ul>

  <h3>۵. مشکلات برداشت بیش از اندازه آب زیرزمینی</h3>
  <div class="answer pink">
    برداشت بی‌رویه از آب‌های زیرزمینی می‌تواند باعث پایین رفتن
    سطح آب زیرزمینی، کاهش ذخایر آب و فرونشست زمین شود.
    به همین دلیل باید در مصرف آب صرفه‌جویی و از منابع زیرزمینی
    محافظت کنیم.
  </div>

  <h3>۶. مقایسه دو منبع آب</h3>
  <table>
    <tr>
      <th>آب‌های سطحی</th>
      <th>آب‌های زیرزمینی</th>
    </tr>
    <tr>
      <td>در رودخانه‌ها و پشت سدها وجود دارند.</td>
      <td>در فضاهای خالی خاک و شکاف سنگ‌ها قرار دارند.</td>
    </tr>
    <tr>
      <td>به بارندگی و ذخیره سدها وابستگی دارند.</td>
      <td>با نفوذ آب در زمین تغذیه می‌شوند.</td>
    </tr>
    <tr>
      <td>با سد و رودخانه قابل دسترسی هستند.</td>
      <td>معمولاً با چاه‌ها برداشت می‌شوند.</td>
    </tr>
  </table>

  <div class="answer green">
    <b>نتیجه تحقیق دوم:</b>
    استان تهران برای تأمین آب از هر دو منبع سطحی و زیرزمینی
    استفاده می‌کند. در آب آشامیدنی شهر تهران، منابع سطحی معمولاً
    سهم بیشتری دارند؛ اما منابع زیرزمینی نیز اهمیت زیادی دارند.
    جمعیت زیاد، بارندگی نامنظم و خشکسالی از دلایل استفاده از هر دو
    منبع هستند.
  </div>
</section>

<!-- نتیجه گیری -->

<section class="lesson" id="result">
  <h2>نتیجه‌گیری نهایی</h2>

  <p>
    آب یکی از مهم‌ترین منابع طبیعی برای ادامه زندگی انسان،
    جانوران و گیاهان است. بارورسازی ابرها می‌تواند در شرایط
    مناسب به افزایش احتمالی بارش کمک کند. همچنین شناخت منابع
    آب سطحی و زیرزمینی و مدیریت درست آن‌ها برای تأمین آب
    مورد نیاز شهرهای بزرگی مانند تهران اهمیت زیادی دارد.
  </p>

  <div class="answer green">
    <b>پیام اصلی تحقیق:</b>
    منابع آب محدود هستند؛ بنابراین همه ما باید در مصرف آب
    مسئولانه رفتار کنیم و از منابع طبیعی محافظت کنیم.
  </div>

  <h3>منابع پیشنهادی برای مطالعه بیشتر</h3>
  <ul>
    <li>سازمان جهانی هواشناسی (WMO)</li>
    <li>سازمان زمین‌شناسی و اکتشافات معدنی کشور</li>
    <li>شرکت آب و فاضلاب استان تهران</li>
    <li>شرکت مدیریت منابع آب ایران</li>
  </ul>
</section>

</main>

<footer>
  <strong>AMIR SG</strong><br>
  پروژه تحقیقات علوم تجربی پایه هفتم<br>
  تهیه و تنظیم: امیرحسین مواظب<br>
  © AMIR SG Educational Project
</footer>

</body>
</html>
