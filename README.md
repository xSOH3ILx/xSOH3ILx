<div align="center">

<img src="assets/header-banner.svg" alt="Soheil Vatandoust - Idea Maker & Software Architect" width="100%" />

<br /><br />

<p align="center">
  <em>I look for simpler, more efficient ways to solve problems and turn fresh ideas into useful, high-impact products. AI is one of the tools I use along the way.</em>
  <br />
  <span dir="rtl" style="display:inline-block;">برای حل مسئله، دنبال راه‌های ساده‌تر و بهینه‌تر می‌گردم و ایده‌های تازه رو به یه محصول کاربردی می‌رسونم. هوش مصنوعی هم یکی از ابزارهاییه که توی این مسیر به کار می‌گیرم.</span>
</p>

<p align="center">
  <a href="https://soheil-vatandoust.ir"><img src="https://img.shields.io/badge/Website-soheil--vatandoust.ir-0969da?style=flat-square&logo=google-chrome&logoColor=white" alt="Website" /></a>
  <a href="https://t.me/Soheil_VatanDoust"><img src="https://img.shields.io/badge/Telegram-@Soheil__VatanDoust-229ED9?style=flat-square&logo=telegram&logoColor=white" alt="Telegram" /></a>
  <a href="https://wa.me/message/7OACOSEAUQLWL1"><img src="https://img.shields.io/badge/WhatsApp-Chat-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="WhatsApp" /></a>
  <a href="mailto:vatandoust.soheil@gmail.com"><img src="https://img.shields.io/badge/Email-vatandoust.soheil@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

</div>

---

### 💡 About Me • درباره من

#### 🇬🇧 English
- 🔭 **Current Focus:** Crafting modern Android solutions, high-performance systems with Go & Rust, resilient web platforms, and intelligent automation.
- 🎯 **Engineering Mindset:** Problem-first thinking, clean architecture, pragmatic design patterns, and high-performance execution across open-source and enterprise products.
- 💬 **Ask me about:** Android (Kotlin & Jetpack Compose), Next.js / TypeScript, Enterprise Backend (FastAPI, Go, Rust), Relational Databases (PostgreSQL, Prisma), and Linux automation.
- ⚡ **Philosophy:** The best software solves complex problems with the simplest, most elegant solution.

<div dir="rtl" align="right">

#### 🇮🇷 درباره من
- 🔭 **تمرکز فعلی:** توسعه راهکارهای مدرن اندروید، سیستم‌های سریع با Go و Rust، معماری وب مقیاس‌پذیر و ربات‌ها و اتوماسیون هوشمند.
- 🎯 **دیدگاه مهندسی:** اولویت حل مسئله، معماری تمیز (Clean Architecture)، الگوهای طراحی کاربردی و مهندسی دقیق در پروژه‌های تجاری و متن‌باز.
- 💬 **گفت‌وگو و همکاری:** اندروید (کاتلین و کامپوز)، فول‌استک (Next.js و تایپ‌اسکریپت)، بک‌اند پیشرفته (FastAPI, Go, Rust)، دیتابیس‌ها (PostgreSQL و Prisma) و سیستم‌های لینوکسی.
- ⚡ **باور من:** بهترین نرم‌افزار، نرم‌افزاریه که مسئله‌ای پیچیده رو با ساده‌ترین و زیباترین راه‌حل ممکن برطرف کنه.

</div>

---

### 🔒 Commercial & Enterprise Work (NDA) • پروژه‌های تجاری و تعهدنامه محرمانگی

> [!NOTE]
> **🇬🇧 Client Work & Non-Disclosure Agreements (NDAs):**
> A substantial share of my day-to-day production code, system architectures, and enterprise engineering resides in **private repositories** for clients and commercial products under strict NDAs. While those proprietary codebases remain strictly confidential, the architectural discipline, clean-code standards, and problem-solving methodology demonstrated across my public repositories reflect the identical high standards applied to all commercial engagements.
> 
> <div dir="rtl" align="right">
> 
> **🇮🇷 پروژه‌های تجاری و تعهدنامه محرمانگی (NDA):**
> بخش عمده‌ای از کدنویسی پروداکشن، معماری سیستم‌ها و پروژه‌های تجاری روزمره من در **مخازن خصوصی** برای کارفرمایان و محصولات تجاری تحت قراردادهای رسمی عدم افشا (NDA) قرار دارد. با حفظ کامل محرمانگی این سورس‌کدها، انضباط معماری، استاندارد کدهای تمیز و شیوه حل مسئله‌ای که در مخازن عمومی مشاهده می‌کنید، بازتاب‌دهنده همان استانداردهای بالا در تمامی پروژه‌های تجاری من است.
> 
> </div>

---

### ⚡ Architectural Case Studies & Engineering Highlights • چالش‌ها و دستاوردهای معماری

<details>
  <summary><b>📱 1. Zero-Drift Solar Engine vs. Android OEM Doze Mode (SOH3IL)</b></summary>
  <br />
  <p><strong>🇬🇧 The Challenge:</strong> Most Android calendars drift reminders by 1–2 days in Persian leap/31-day months, while aggressive vendor battery managers (Xiaomi, Samsung) kill background alarms.</p>
  <p><strong>The Architecture:</strong></p>
  <ul>
    <li>Rules stored natively in Solar Jalali format (<code>RecurrenceRule</code>) in Room SQLite.</li>
    <li><code>AlarmManager.setAlarmClock()</code> triggers CPU wake-up exactly on target second with zero battery penalty during idle hours.</li>
    <li>Deterministic <code>SNAP_TO_LAST_DAY</code> policy for Esfand and 30-day months.</li>
  </ul>
  
  <div dir="rtl" align="right">
    <p><strong>🇮🇷 چالش فنی:</strong> جابجایی ۱ الی ۲ روزه یادآورهای دوره‌ای خورشیدی در ماه‌های ۳۱ و ۲۹ روزه، همراه با بسته شدن پروسه‌های پس‌زمینه توسط مدیریت باتری گوشی‌ها.</p>
    <p><strong>راه‌حل معماری:</strong></p>
    <ul>
      <li>ذخیره بومی الگوهای تکرار با تقویم جلالی در Room دیتابیس بدون تبدیل مبنا به میلادی.</li>
      <li>استفاده از <code>AlarmManager.setAlarmClock()</code> برای بیداری دقیق پردازنده با مصرف باتری صفر در زمان خواب دستگاه.</li>
      <li>سیاست انطباق هوشمند <code>SNAP_TO_LAST_DAY</code> برای انطباق خودکار یادآورهای روز ۳۱ در ماه‌های ۳۰ روزه و اسفند.</li>
    </ul>
  </div>
</details>

<details>
  <summary><b>🤖 2. Serverless Telegram Rich Messaging at Global Edge Latency (TeleRich Studio)</b></summary>
  <br />
  <p><strong>🇬🇧 The Challenge:</strong> Parsing complex Markdown/HTML ASTs, rendering live previews, and managing Telegram Bot API 10.3 entities without running an expensive dedicated server.</p>
  <p><strong>The Architecture:</strong></p>
  <ul>
    <li>Compiled full studio engine on <strong>Cloudflare Workers</strong> (0ms cold start, sub-50ms edge latency worldwide).</li>
    <li>State persistence, webhook rate-limiting, and draft sessions managed via <strong>Durable Objects + SQLite storage</strong>.</li>
    <li>Private media assets served and buffered via <strong>Cloudflare R2</strong> bucket bindings.</li>
  </ul>

  <div dir="rtl" align="right">
    <p><strong>🇮🇷 چالش فنی:</strong> پردازش درخت گرامری (AST) متن‌های پیچیده Markdown/HTML، پیش‌نمایش بلادرنگ و انتشار بر اساس Bot API 10.3 بدون نیاز به اجاره سرورهای گران‌قیمت.</p>
    <p><strong>راه‌حل معماری:</strong></p>
    <ul>
      <li>استقرار کامل موتور پردازش روی <strong>Cloudflare Workers</strong> با کلد استارت صفر ثانیه و تاخیر زیر ۵۰ میلی‌ثانیه جهانی.</li>
      <li>مدیریت پیش‌نویس‌ها، سشن‌های چندکاربره و ریت‌لیمیت با <strong>Durable Objects بر بستر SQLite داخلی</strong>.</li>
      <li>مدیریت بهینه فایل‌ها و عکس‌های پیام با بایندینگ بومی <strong>Cloudflare R2 Storage</strong>.</li>
    </ul>
  </div>
</details>

<details>
  <summary><b>📈 3. High-Throughput Quantitative Microstructure & Liquidity Engine (SmartMoney-Analyst)</b></summary>
  <br />
  <p><strong>🇬🇧 The Challenge:</strong> Real-time processing of massive orderbook ticks and algorithmic detection of institutional liquidity sweeps without garbage-collection pauses.</p>
  <p><strong>The Architecture:</strong></p>
  <ul>
    <li>Engineered core analysis pipeline in <strong>Rust</strong> using zero-cost abstractions and lock-free ring buffers.</li>
    <li>Sub-millisecond market microstructure parsing and imbalance volume profiling.</li>
    <li>Seamless integration with asynchronous Python/FastAPI downstream services for alert distribution.</li>
  </ul>

  <div dir="rtl" align="right">
    <p><strong>🇮🇷 چالش فنی:</strong> پردازش بلادرنگ جریان سفارشات (Orderbook) و شناسایی نقدینگی نهادی بازارهای مالی بدون افت پرفورمنس ناشی از Garbage Collection.</p>
    <p><strong>راه‌حل معماری:</strong></p>
    <ul>
      <li>طراحی پایپ‌لاین هسته پردازشی با زبان <strong>Rust</strong> و بهره‌گیری از Zero-Cost Abstractions و بافرهای غیرمسدودکننده (Lock-Free).</li>
      <li>محاسبه آنی حجم و جریان نقدینگی در مقیاس زیر میلی‌ثانیه.</li>
      <li>ارتباط ساخت‌یافته با سرویس‌های ناهمگام Python/FastAPI جهت توزیع بلادرنگ هشدارهای معاملاتی.</li>
    </ul>
  </div>
</details>

---

### 📈 Enterprise & Development Footprint • کارنامه و ردپای فنی پروژه‌ها

<table>
  <tr>
    <td align="center" width="25%">
      <h3>۱۹</h3>
      <p><strong>Active Repositories</strong><br /><small dir="rtl">مجموع مخازن فعال</small></p>
    </td>
    <td align="center" width="25%">
      <h3>Multi-Stack</h3>
      <p><strong>Systems Architecture</strong><br /><small dir="rtl">معماری سیستم‌های چندسکویی</small></p>
    </td>
    <td align="center" width="25%">
      <h3>۹</h3>
      <p><strong>Enterprise NDA Repos</strong><br /><small dir="rtl">پروژه‌های تجاری و محرمانه</small></p>
    </td>
    <td align="center" width="25%">
      <h3>۱۰</h3>
      <p><strong>Open Source Repos</strong><br /><small dir="rtl">پروژه‌ها و ابزارهای متن‌باز</small></p>
    </td>
  </tr>
</table>

<details>
  <summary><b>🔍 Architectural Track Record by Domain • تفکیک حوزه‌های تخصصی پروژه‌ها</b></summary>
  <br />
  <table>
    <tr>
      <td width="30%"><strong>TypeScript &amp; JavaScript</strong></td>
      <td width="30%"><img src="https://img.shields.io/badge/Ecosystem-Full--Stack-3178C6?style=flat-square" alt="TypeScript" /></td>
      <td><small dir="rtl">پلتفرم‌های جامع سازمانی، Next.js 16، React 19، PWA و کلودفلر</small></td>
    </tr>
    <tr>
      <td><strong>Python &amp; FastAPI</strong></td>
      <td><img src="https://img.shields.io/badge/Ecosystem-Microservices-3776AB?style=flat-square" alt="Python" /></td>
      <td><small dir="rtl">معماری میکروسرویس‌ها، موتورهای محاسباتی و APIهای پرسرعت</small></td>
    </tr>
    <tr>
      <td><strong>Go (Golang) &amp; Rust</strong></td>
      <td><img src="https://img.shields.io/badge/Ecosystem-High--Performance-00ADD8?style=flat-square" alt="Go and Rust" /></td>
      <td><small dir="rtl">سیستم‌های عملکرد بالا، پردازش تراکنش‌ها و تحلیل میکرواستراکچر مالی</small></td>
    </tr>
    <tr>
      <td><strong>Kotlin &amp; Android</strong></td>
      <td><img src="https://img.shields.io/badge/Ecosystem-Native_Mobile-7F52FF?style=flat-square" alt="Kotlin" /></td>
      <td><small dir="rtl">اپلیکیشن‌های نیتیو اندروید، جت‌پک کامپوز و سیستم‌های یادآور خورشیدی</small></td>
    </tr>
    <tr>
      <td><strong>SQL &amp; PostgreSQL</strong></td>
      <td><img src="https://img.shields.io/badge/Ecosystem-Relational_Data-336791?style=flat-square" alt="SQL" /></td>
      <td><small dir="rtl">مدل‌سازی رابطه‌ای دیتابیس، مایگریشن‌ها و کوئری‌های بهینه با Prisma</small></td>
    </tr>
  </table>
</details>

---

### 🚀 Featured Open Source Projects • پروژه‌های شاخص متن‌باز

<table>
  <tr>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/xSOH3ILx/SOH3IL">📱 SOH3IL</a></h4>
      <p>Modern Persian Jalali Calendar & Exact Solar Recurring Reminder Engine for Android built with Kotlin and Jetpack Compose.</p>
      <div dir="rtl" align="right">
        <p><small>تقویم جلالی مدرن و موتور پردازش یادآورهای دقیق خورشیدی برای اندروید، پیاده‌سازی‌شده با کاتلین و جت‌پک کامپوز.</small></p>
      </div>
      <p>
        <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" />
        <img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white" />
        <img src="https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" />
      </p>
    </td>
    <td width="50%" valign="top">
      <h4><a href="https://github.com/xSOH3ILx/TeleRich-Standalone">🤖 TeleRich-Standalone</a></h4>
      <p>Independent Telegram Rich Messaging Studio & bot engine running serverless on Cloudflare Workers with native Markdown/HTML live rendering.</p>
      <div dir="rtl" align="right">
        <p><small>استودیو و ربات مستقل پیام‌رسانی پیشرفته تلگرام (Rich Messaging) مبتنی بر کلودفلر ورکرز با رندر زنده Markdown و HTML.</small></p>
      </div>
      <p>
        <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
        <img src="https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white" />
        <img src="https://img.shields.io/badge/Telegram_Bot-24A1DE?style=flat-square&logo=telegram&logoColor=white" />
      </p>
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <h4><a href="https://github.com/xSOH3ILx/Gnome-PersianCalendar">🐧 Gnome-PersianCalendar</a></h4>
      <p>Persian (Jalali) Solar Calendar integration and indicator for the GNOME Shell desktop environment on Linux.</p>
      <div dir="rtl" align="right">
        <p><small>افزونه و نشانگر تقویم خورشیدی جلالی برای میزکار لینوکس GNOME Shell.</small></p>
      </div>
      <p>
        <img src="https://img.shields.io/badge/GNOME-4A86CF?style=flat-square&logo=gnome&logoColor=white" />
        <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
        <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
      </p>
    </td>
  </tr>
</table>

---

### 🛠️ Tech Stack & Architecture • جعبه‌ابزار و معماری فنی

<table>
  <tr>
    <td align="right" width="28%"><strong>Mobile • موبایل</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white" alt="Android" />
      <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin" />
      <img src="https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" />
      <img src="https://img.shields.io/badge/Material_Design_3-757575?style=flat-square&logo=material-design&logoColor=white" alt="M3" />
    </td>
  </tr>
  <tr>
    <td align="right" width="28%"><strong>Web & Full-Stack • فرانت‌اند</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Next.js_16-000000?style=flat-square&logo=next.js&logoColor=white" alt="Next.js" />
      <img src="https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React" />
      <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
      <img src="https://img.shields.io/badge/Vue.js-35495E?style=flat-square&logo=vue.js&logoColor=4FC08D" alt="Vue" />
      <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind" />
    </td>
  </tr>
  <tr>
    <td align="right" width="28%"><strong>Backend & Systems • بک‌اند و سیستم</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
      <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" alt="FastAPI" />
      <img src="https://img.shields.io/badge/Go_(Golang)-00ADD8?style=flat-square&logo=go&logoColor=white" alt="Go" />
      <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
      <img src="https://img.shields.io/badge/Linux_/_Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white" alt="Linux" />
    </td>
  </tr>
  <tr>
    <td align="right" width="28%"><strong>Databases & ORM • پایگاه‌های داده</strong></td>
    <td>
      <img src="https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
      <img src="https://img.shields.io/badge/Prisma_ORM-2D3748?style=flat-square&logo=prisma&logoColor=white" alt="Prisma" />
      <img src="https://img.shields.io/badge/SQLite-07405E?style=flat-square&logo=sqlite&logoColor=white" alt="SQLite" />
      <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
    </td>
  </tr>
  <tr>
    <td align="right" width="28%"><strong>Cloud & DevOps • زیرساخت و ابری</strong></td>
    <td>
      <img src="https://img.shields.io/badge/Cloudflare_Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white" alt="Cloudflare" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
      <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
      <img src="https://img.shields.io/badge/Telegram_Bot_API-24A1DE?style=flat-square&logo=telegram&logoColor=white" alt="Telegram API" />
    </td>
  </tr>
</table>

---

### 📊 GitHub Activity & Dynamics • پویایی فعالیت‌های گیت‌هاب

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/xSOH3ILx/xSOH3ILx/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/xSOH3ILx/xSOH3ILx/output/github-contribution-grid-snake.svg" />
    <img alt="GitHub Contribution Snake" src="https://raw.githubusercontent.com/xSOH3ILx/xSOH3ILx/output/github-contribution-grid-snake-dark.svg" width="100%" />
  </picture>
</div>

---

<div align="center">
  <sub>Designed with precision & craftsmanship • طراحی‌شده با ظرافت و دقت مهندسی • © 2026 Soheil Vatandoust</sub>
</div>
