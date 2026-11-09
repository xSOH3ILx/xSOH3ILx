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

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>🇬🇧 English</h4>
      <ul>
        <li>🔭 <b>Current Focus:</b> Crafting modern Android solutions, high-performance systems with Go & Rust, resilient web architectures, and intelligent automation.</li>
        <li>🎯 <b>Engineering Mindset:</b> Problem-first thinking, clean architecture, pragmatic design patterns, and high-performance execution across open-source and enterprise products.</li>
        <li>💬 <b>Ask me about:</b> Android (Kotlin & Jetpack Compose), Next.js / TypeScript, Enterprise Backend (FastAPI, Go, Rust), Relational Databases (PostgreSQL, Prisma), and Linux automation.</li>
        <li>⚡ <b>Philosophy:</b> The best software solves complex problems with the simplest, most elegant solution.</li>
      </ul>
    </td>
    <td width="50%" valign="top" dir="rtl" align="right">
      <div dir="rtl" align="right">
        <h4>🇮🇷 فارسی</h4>
        <ul>
          <li>🔭 <b>تمرکز فعلی:</b> توسعه راهکارهای مدرن اندروید، سیستم‌های سریع با Go و Rust، معماری وب مقیاس‌پذیر و ربات‌ها و اتوماسیون هوشمند.</li>
          <li>🎯 <b>دیدگاه مهندسی:</b> اولویت حل مسئله، معماری تمیز (Clean Architecture)، الگوهای طراحی کاربردی و مهندسی دقیق در پروژه‌های تجاری و متن‌باز.</li>
          <li>💬 <b>گفت‌وگو و همکاری:</b> اندروید (کاتلین و کامپوز)، فول‌استک (Next.js و تایپ‌اسکریپت)، بک‌اند پیشرفته (FastAPI, Go, Rust)، دیتابیس‌ها (PostgreSQL و Prisma) و سیستم‌های لینوکسی.</li>
          <li>⚡ <b>باور من:</b> بهترین نرم‌افزار، نرم‌افزاریه که مسئله‌ای پیچیده رو با ساده‌ترین و زیباترین راه‌حل ممکن برطرف کنه.</li>
        </ul>
      </div>
    </td>
  </tr>
</table>

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
  <table>
    <tr>
      <td width="50%" valign="top">
        <p><strong>The Challenge:</strong> Most Android calendars drift reminders by 1–2 days in Persian leap/31-day months, while aggressive vendor battery managers (Xiaomi, Samsung) kill background alarms.</p>
        <p><strong>The Architecture:</strong></p>
        <ul>
          <li>Rules stored natively in Solar Jalali format (<code>RecurrenceRule</code>) in Room SQLite.</li>
          <li><code>AlarmManager.setAlarmClock()</code> triggers CPU wake-up exactly on target second with zero battery penalty during idle hours.</li>
          <li>Deterministic <code>SNAP_TO_LAST_DAY</code> policy for Esfand and 30-day months.</li>
        </ul>
      </td>
      <td width="50%" valign="top" dir="rtl" align="right">
        <div dir="rtl" align="right">
          <p><strong>چالش فنی:</strong> جابجایی ۱ الی ۲ روزه یادآورهای دوره‌ای خورشیدی در ماه‌های ۳۱ و ۲۹ روزه، همراه با بسته شدن پروسه‌های پس‌زمینه توسط مدیریت باتری گوشی‌ها.</p>
          <p><strong>راه‌حل معماری:</strong></p>
          <ul>
            <li>ذخیره بومی الگوهای تکرار با تقویم جلالی در Room دیتابیس بدون تبدیل مبنا به میلادی.</li>
            <li>استفاده از <code>AlarmManager.setAlarmClock()</code> برای بیداری دقیق پردازنده با مصرف باتری صفر در زمان خواب دستگاه.</li>
            <li>سیاست انطباق هوشمند <code>SNAP_TO_LAST_DAY</code> برای انطباق خودکار یادآورهای روز ۳۱ در ماه‌های ۳۰ روزه و اسفند.</li>
          </ul>
        </div>
      </td>
    </tr>
  </table>
</details>

<details>
  <summary><b>🤖 2. Serverless Telegram Rich Messaging at Global Edge Latency (TeleRich Studio)</b></summary>
  <br />
  <table>
    <tr>
      <td width="50%" valign="top">
        <p><strong>The Challenge:</strong> Parsing complex Markdown/HTML ASTs, rendering live previews, and managing Telegram Bot API 10.3 entities without running an expensive dedicated server.</p>
        <p><strong>The Architecture:</strong></p>
        <ul>
          <li>Compiled full studio engine on <strong>Cloudflare Workers</strong> (0ms cold start, sub-50ms edge latency worldwide).</li>
          <li>State persistence, webhook rate-limiting, and draft sessions managed via <strong>Durable Objects + SQLite storage</strong>.</li>
          <li>Private media assets served and buffered via <strong>Cloudflare R2</strong> bucket bindings.</li>
        </ul>
      </td>
      <td width="50%" valign="top" dir="rtl" align="right">
        <div dir="rtl" align="right">
          <p><strong>چالش فنی:</strong> پردازش درخت گرامری (AST) متن‌های پیچیده Markdown/HTML، پیش‌نمایش بلادرنگ و انتشار بر اساس Bot API 10.3 بدون نیاز به اجاره سرورهای گران‌قیمت.</p>
          <p><strong>راه‌حل معماری:</strong></p>
          <ul>
            <li>استقرار کامل موتور پردازش روی <strong>Cloudflare Workers</strong> با کلد استارت صفر ثانیه و تاخیر زیر ۵۰ میلی‌ثانیه جهانی.</li>
            <li>مدیریت پیش‌نویس‌ها، سشن‌های چندکاربره و ریت‌لیمیت با <strong>Durable Objects بر بستر SQLite داخلی</strong>.</li>
            <li>مدیریت بهینه فایل‌ها و عکس‌های پیام با بایندینگ بومی <strong>Cloudflare R2 Storage</strong>.</li>
          </ul>
        </div>
      </td>
    </tr>
  </table>
</details>

<details>
  <summary><b>📈 3. High-Throughput Quantitative Microstructure & Liquidity Engine (SmartMoney-Analyst)</b></summary>
  <br />
  <table>
    <tr>
      <td width="50%" valign="top">
        <p><strong>The Challenge:</strong> Real-time processing of massive orderbook ticks and algorithmic detection of institutional liquidity sweeps without garbage-collection pauses.</p>
        <p><strong>The Architecture:</strong></p>
        <ul>
          <li>Engineered core analysis pipeline in <strong>Rust</strong> using zero-cost abstractions and lock-free ring buffers.</li>
          <li>Sub-millisecond market microstructure parsing and imbalance volume profiling.</li>
          <li>Seamless integration with asynchronous Python/FastAPI downstream services for alert distribution.</li>
        </ul>
      </td>
      <td width="50%" valign="top" dir="rtl" align="right">
        <div dir="rtl" align="right">
          <p><strong>چالش فنی:</strong> پردازش بلادرنگ جریان سفارشات (Orderbook) و شناسایی نقدینگی نهادی بازارهای مالی بدون افت پرفورمنس ناشی از Garbage Collection.</p>
          <p><strong>راه‌حل معماری:</strong></p>
          <ul>
            <li>طراحی پایپ‌لاین هسته پردازشی با زبان <strong>Rust</strong> و بهره‌گیری از Zero-Cost Abstractions و بافرهای غیرمسدودکننده (Lock-Free).</li>
            <li>محاسبه آنی حجم و جریان نقدینگی در مقیاس زیر میلی‌ثانیه.</li>
            <li>ارتباط ساخت‌یافته با سرویس‌های ناهمگام Python/FastAPI جهت توزیع بلادرنگ هشدارهای معاملاتی.</li>
          </ul>
        </div>
      </td>
    </tr>
  </table>
</details>

---

### 📈 Enterprise & Development Footprint • کارنامه و ردپای فنی پروژه‌ها

<table>
  <tr>
    <td align="center" width="25%">
      <h3>۱۹</h3>
      <p><strong>Total Repositories</strong><br /><small dir="rtl">مجموع مخازن توسعه‌یافته</small></p>
    </td>
    <td align="center" width="25%">
      <h3>15+ MB</h3>
      <p><strong>Production Codebases</strong><br /><small dir="rtl">کدنویسی سورس پروداکشن</small></p>
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
  <summary><b>🔍 Verified Production Language Footprint • جزئیات تفکیکی حجم کدنویسی در مخازن</b></summary>
  <br />
  <table>
    <tr>
      <td width="30%"><strong>TypeScript & JavaScript</strong></td>
      <td width="40%"><img src="https://img.shields.io/badge/Volume-10.5%2B_MB-3178C6?style=flat-square" alt="TypeScript Volume" /></td>
      <td><small dir="rtl">پلتفرم‌های جامع سازمانی، Next.js 16، React 19، PWA و کلودفلر</small></td>
    </tr>
    <tr>
      <td><strong>Python & FastAPI</strong></td>
      <td><img src="https://img.shields.io/badge/Volume-3.1%2B_MB-3776AB?style=flat-square" alt="Python Volume" /></td>
      <td><small dir="rtl">معماری میکروسرویس‌ها، موتورهای محاسباتی و APIهای پرسرعت</small></td>
    </tr>
    <tr>
      <td><strong>Go (Golang) & Rust</strong></td>
      <td><img src="https://img.shields.io/badge/Volume-1.0%2B_MB-00ADD8?style=flat-square" alt="Go and Rust Volume" /></td>
      <td><small dir="rtl">سیستم‌های عملکرد بالا، پردازش تراکنش‌ها و ابزارهای تحلیلی مالی</small></td>
    </tr>
    <tr>
      <td><strong>Kotlin & Android</strong></td>
      <td><img src="https://img.shields.io/badge/Volume-630%2B_KB-7F52FF?style=flat-square" alt="Kotlin Volume" /></td>
      <td><small dir="rtl">اپلیکیشن‌های نیتیو اندروید، جت‌پک کامپوز و سیستم‌های یادآور خورشیدی</small></td>
    </tr>
    <tr>
      <td><strong>SQL & PostgreSQL (PLpgSQL)</strong></td>
      <td><img src="https://img.shields.io/badge/Database-Schemas_&_Migrations-336791?style=flat-square" alt="SQL Volume" /></td>
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

### 📊 GitHub Activity & Statistics • آمار فعالیت

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=xSOH3ILx&show_icons=true&count_private=true&hide_border=true&theme=tokyonight&title_color=58a6ff&text_color=c9d1d9&icon_color=58a6ff&bg_color=0d1117" alt="Soheil's GitHub Stats" height="165" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=xSOH3ILx&hide_border=true&theme=tokyonight&ring=58a6ff&fire=58a6ff&currStreakNum=58a6ff&sideNums=c9d1d9&currStreakLabel=58a6ff&sideLabels=c9d1d9&dates=8b949e&background=0d1117" alt="GitHub Streak" height="165" />
</div>

<br />

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
