# [عنوان]

| فیلد | مقدار |
|---|---|
| Target release | Name |
| Document owner |  |
| Designer |  |
| PM |  |
| Status | DRAFT |
| Developers |  |
| Related Docs |  |

## مشکل و زمینه (Problem / Context)

### In Context

وضعیت فعلی سیستم را توضیح دهید:

- رفتار واقعی کاربر، نه فرضیه درباره رفتار او
- محدودیت‌های فعلی محصول، فنی یا عملیاتی
- شرایطی که مسئله در آن رخ می‌دهد
- Evidence و لینک منبع، در صورت وجود

در این بخش راه‌حل پیشنهاد ندهید.

### In Problem

Problem باید روی Business Pain یا User Pain تمرکز کند، نه Feature. آن را ترجیحاً در یک جمله واضح بنویسید و impact را مشخص کنید؛ مانند ریسک، خطا، drop، کاهش revenue، کاهش adoption، retention پایین یا funnel drop.

نوع Problem را مشخص کنید:

- User pain: کاربر مستقیماً با مشکل مواجه است.
- Business impact: یک Metric یا نتیجه کسب‌وکار آسیب دیده است.
- Opportunity gap: قابلیتی یا تجربه‌ای وجود ندارد که باید وجود داشته باشد.
- Competitive gap: بازار یا رقبا تجربه بهتری ارائه می‌کنند.

Problem بدون Evidence معتبر نیست. اگر Evidence وجود ندارد، آن را با یکی از وضعیت‌های `Not provided`، `Not available` یا `Needs validation` ثبت کنید.

## Goals & Non-Goals

### Goals

- User outcome: کاربر بعد از این کار چه چیزی را بهتر انجام می‌دهد؟
- Business outcome: کدام Metric یا هدف کسب‌وکار باید بهبود پیدا کند؟
- Success direction: انتظار داریم چه تغییری رخ دهد؟
- Scope boundary: این نسخه اول تا کجا پیش می‌رود؟

### Non-Goals

- قابلیت‌هایی که به فاز بعد موکول شده‌اند
- Edge caseهایی که فعلاً پشتیبانی نمی‌شوند
- تغییرات بزرگ Product-wide که به این کار مرتبط نیستند
- بهبودهای جانبی که مفیدند اما در این نسخه Priority ندارند

## Success Metrics

### Primary Metrics

| Metric | Baseline | Target | Timeframe | Data Source | Owner |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

### Secondary Metrics (Guardrails)

| Metric | Baseline | Target | Timeframe | Data Source | Owner |
|---|---|---|---|---|---|
|  |  |  |  |  |  |

اگر Metric یا یکی از فیلدهای آن مشخص نیست، مقدار را حدس نزنید و وضعیت آن را ثبت کنید.

## Research & Insights

### User insights

یافته‌های مستقیم از کاربران، مصاحبه‌ها، تست‌ها، فیدبک‌ها یا تیکت‌های پشتیبانی را ثبت کنید. بین مشاهده مستقیم و تفسیر تیم تفاوت بگذارید.

### Analytics

داده‌های محصول، رفتار کاربران، تعریف Metric، بازه زمانی، جامعه بررسی‌شده و لینک تحلیل را ثبت کنید.

### Benchmarks

Benchmarkهای داخلی، خارجی یا رقابتی را همراه با دامنه بررسی، لینک منبع، لینک Figma، Notes و نتیجه تحلیل ثبت کنید. اگر Benchmark در Figma مستند شده است، نام File، Page، Section یا Frame بررسی‌شده را هم بنویسید.

#### دامنه بررسی

- چه محصول، رقیب یا الگوهایی بررسی شدند؟
- چرا این موارد برای این مسئله انتخاب شدند؟
- چه بخش‌هایی بررسی شدند؟ مانند Flow، Layout، Information architecture، Component یا Interaction
- لینک Figma، فایل تحلیل یا منبع اصلی چیست؟

#### یافته‌های Benchmark

| مورد بررسی | محصول / رقیب | بخش یا الگوی بررسی‌شده | Observation | Note / Annotation | لینک Figma یا منبع | اثر بر تصمیم طراحی |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |

#### نتیجه حاصل از بررسی

خلاصه کنید که از Benchmarkها چه چیزی کشف شد، کدام الگوها تکرار شدند، چه تفاوتی میان محصولات وجود داشت و این یافته‌ها چه اثری بر Goals، Design Exploration یا Design Solution گذاشتند.

اگر Figma قابل‌دسترسی نیست، وضعیت آن را شفاف ثبت کنید: `Not accessible`، `Not provided` یا `Needs validation`.

## Design Exploration

نشان دهید چه Optionهایی بررسی شده‌اند، چرا بعضی از آن‌ها Reject شده‌اند و چرا Solution نهایی انتخاب شده است.

| Option | توضیح | Pros | Cons | محدودیت یا Evidence مرتبط | تصمیم | لینک Design / Figma |
|---|---|---|---|---|---|---|
|  |  |  |  |  |  |  |

### Iterations

تغییرات مهم در مسیر طراحی را ثبت کنید:

| Iteration | چه چیزی تغییر کرد؟ | چرا تغییر کرد؟ | نتیجه | لینک Design / Figma |
|---|---|---|---|---|
|  |  |  |  |  |

## UX Flow

User journey یا User flow را از نقطه شروع تا پایان توضیح دهید. مسیر اصلی، مسیرهای جایگزین، خطاها و حالت‌های خروج را در صورت مرتبط‌بودن نشان دهید.

```text
[Entry point] → [Action] → [Decision / state] → [Outcome]
```

لینک Flow، Prototype یا Figma را اینجا قرار دهید.

## Design Solution

### Screens

Screenهای طراحی‌شده، نقش هر Screen و لینک مربوط به آن را ثبت کنید.

### Key components

Componentهای اصلی و نقش آن‌ها را ثبت کنید.

### Layout decisions

تصمیم‌های مربوط به Layout، hierarchy، responsive behavior و محدودیت‌های نمایش را با دلیل ثبت کنید.

### Interaction Details

رفتار تعاملی هر Screen یا بخش مهم را توضیح دهید. جزئیات کامل را در بخش Interaction Details ثبت کنید.

### Empty States

برای هر Empty State، شرایط نمایش، متن، Action و لینک Design را ثبت کنید.

### Error States

برای هر Error State، اتفاق رخ‌داده، علت قابل‌نمایش، راه برگشت و متن پیشنهادی را ثبت کنید.

### Alternatives Considered

Alternativeهایی را ثبت کنید که در مرحله Solution بررسی شدند اما انتخاب نشدند. اگر در Design Exploration آمده‌اند، به آن بخش ارجاع دهید.

### Edge Cases

Edge caseهای پشتیبانی‌شده، Deferred و Unsupported را از هم جدا کنید.

## Interaction Details

### Behaviors

رفتارهای مورد انتظار در حالت‌های مختلف، تغییر وضعیت، Loading، Success، Warning و Error را ثبت کنید.

### Micro-interactions

Micro-interactionها، feedbackها، transitionها و triggerهای آن‌ها را همراه با لینک Prototype یا Figma ثبت کنید.

## Component / Spec

### Component anatomy

ساختار داخلی Component و بخش‌های تشکیل‌دهنده آن را توضیح دهید.

### Variants

Variantها، حالت‌های مختلف و شرایط استفاده از هرکدام را ثبت کنید.

### Rules

قواعد استفاده، محدودیت‌ها، وابستگی‌ها، responsive behavior و شرایط reuse را ثبت کنید.

## Open Questions

Open Questions ابهام‌های مهمی هستند که هنوز پاسخ روشنی ندارند، اما می‌توانند بر تصمیمات طراحی، محدوده یا نتایج تأثیر بگذارند.

آن‌ها ناشناخته‌ها را قابل مشاهده می‌کنند و به تیم کمک می‌کنند قبل از حرکت به جلو، از فرضیات و ریسک‌ها آگاه باشد.

### هدف

- شناسایی زودهنگام شکاف‌های دانش
- جلوگیری از فرضیات پنهان
- هماهنگ‌کردن تیم درباره چیزهایی که هنوز نامشخص هستند
- فعال‌کردن تصمیم‌گیری آگاهانه در شرایط عدم قطعیت

| Question | چرا مهم است؟ | اثر احتمالی | Owner | Next action | Status |
|---|---|---|---|---|---|
|  |  |  |  |  | Open |

## Post-Launch

بعد از Launch این موارد را بررسی کنید:

- آیا Hypothesis درست بود؟
- User behavior واقعی چه بود؟
- چه چیزی کار نکرد؟
- کدام Metric تغییر کرد؟
- چه Iterationای لازم است؟
- چه شواهدی باعث بازشدن دوباره این تصمیم می‌شود؟

| بررسی | Signal / Metric | Data Source | زمان بررسی | Owner | نتیجه |
|---|---|---|---|---|---|
|  |  |  |  |  |  |
