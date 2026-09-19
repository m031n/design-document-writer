# Farsi product-document writing style

این راهنما از الگوهای نگارشی [persian-writing](https://github.com/ali2000hos/persian-writing) استفاده می‌کند و برای سندهای Product Design تنظیم شده است. هدف، فارسی روان و دقیق است؛ نه محاوره‌ای‌کردن اجباری متن و نه تلاش برای عبور از ابزارهای تشخیص متن ماشینی.

## انتخاب لحن پیش از نوشتن

لحن را بر اساس **نوع سند و مخاطب** انتخاب کنید، نه لحن پیام کاربر. این سند برای Product Designer و Product Manager نوشته می‌شود و پیش‌فرض آن `formal-but-human` است:

- جمله‌ها رسمی و کامل باشند: «می‌شود»، نه «میشه»؛ «است»، نه «می‌باشد».
- متن مستقیم و زنده باشد، اما به محاوره، تعارف اداری یا عبارت‌های کتابی نلغزد.
- اگر خروجی برای کاربر نهایی است، لحن UI را از لحن مستندات جدا کنید و آن را با UX-writing هماهنگ کنید.
- اگر نوع مخاطب یا مقصد سند لحن را تغییر می‌دهد و اطلاعات کافی نداریم، یک سؤال کوتاه بپرسید؛ حدس‌زدن لحن در سندی که برای شخص ثالث ارسال می‌شود قابل‌قبول نیست.

در این نوع سند، سه سطح را از هم جدا نگه دارید:

1. **واقعیت و مکانیزم:** لحن خنثی و دقیق؛ مانند «کاربر وارد صفحه جزئیات می‌شود».
2. **تفسیر و تصمیم تیم:** فاعل مشخص داشته باشد؛ مانند «این یافته، بررسی Filter را به یک Design Question تبدیل می‌کند».
3. **متن UI:** کوتاه، عملی و متناسب با سطح رسمی محصول؛ مانند «مشاهده تاریخچه».

## زاویه دید

- برای واقعیت‌ها و مکانیزم‌ها از بیان خنثی استفاده کنید.
- برای کاری که کاربر انجام می‌دهد، فعل مستقیم کافی است؛ تکرار «کاربر می‌تواند» در هر جمله متن را ترجمه‌ای می‌کند.
- «ما» را فقط برای اقدام یا مسئولیت واقعی تیم به‌کار ببرید؛ مانند «در Benchmark سه رقیب را بررسی کردیم».
- بین بیان خنثی، خطاب مستقیم و «ما» بدون دلیل جابه‌جا نشوید.

## Voice

Write in simple, direct, professional Farsi for Product Designers and Product Managers. Use English product terms when they are clearer or are the team’s established terminology. Do not translate names of tools, components, metrics, or concepts into awkward Persian equivalents.

Use one professional register throughout the document. The default is formal-but-human product writing unless the author supplies another voice sample.

Prefer:

- concrete facts over broad claims;
- short, clear sentences with occasional longer explanations when the relationship matters;
- varied rhythm caused by real content, not manufactured informality;
- active voice when the actor is known;
- consistent terminology over forced synonym variety;
- neutral descriptions over promotional language;
- explicit uncertainty over confident speculation;
- concrete verbs such as «است»، «شد» و «کرد» instead of «می‌باشد»، «گردید» و «به عمل آورد».

Avoid:

- bureaucratic fillers such as «لازم به ذکر است»، «شایان ذکر است»، «در راستای» and «به‌طور کلی» when they add no information;
- inflated words such as «انقلابی»، «بی‌نظیر» and «بسیار مهم» without Evidence;
- vague attribution such as «کاربران معتقدند» without naming the source or research;
- generic introductions and repeated conclusions;
- artificial three-item lists and negative parallelism such as «نه‌تنها ... بلکه ...»;
- appended analysis such as «که نشان‌دهنده اهمیت ... است» when the evidence and interpretation should be separate sentences;
- translationese such as «نگاهی بیندازیم به» when a natural Persian verb is available;
- unsupported causal claims;
- turning a design preference into a user finding;
- changing a number, link, product name, or technical term during editing.

## Evidence language

Use precise labels:

- `Evidence`: «داده‌های ۳۰ روز اخیر نشان داد...»
- `Observation`: «در مصاحبه‌ها، چهار کاربر...»
- `Interpretation`: «این داده احتمالاً نشان می‌دهد...»
- `Assumption`: «فرض فعلی تیم این است...»
- `Needs validation`: «برای این ادعا Evidence کافی ثبت نشده است.»

Distinguish four kinds of statement:

- **واقعیت:** مستقیم از منبع یا مشاهده می‌آید.
- **نظر:** قضاوت یا ترجیح تیم است.
- **پیش‌بینی:** انتظار آینده‌نگر است و باید به‌عنوان Hypothesis نوشته شود.
- **ادعا:** نیازمند Evidence یا وضعیت `Needs validation` است.

اگر دو منبع با هم ناسازگارند، تناقض را ثبت کنید و خودسرانه یکی را حذف نکنید. Do not use a strong sentence such as «این تغییر باعث افزایش adoption می‌شود» unless the source supports that level of certainty. Use «هدف این تغییر، افزایش adoption است» when it is only a goal.

## Product and UX writing

When writing UI copy or interaction details:

- use clear action labels, usually Verb + object;
- make destructive actions explicit;
- explain what happened, why it happened, and the next step in errors;
- give empty states a useful next action when one exists;
- keep confirmation text transparent about consequences;
- avoid blaming the user and avoid technical error codes in user-facing copy;
- keep copy short enough for the intended surface and check mobile truncation when relevant.

## Persian consistency pass

Before the deeper edit, normalize the surface form:

- use Persian letters `ی` and `ک`, not mixed Arabic `ي` and `ك`;
- use نیم‌فاصله consistently, such as `می‌شود`، `به‌روزرسانی` and `قابل‌مشاهده`;
- use Persian punctuation such as `،`، `؛`، `؟` and `«»` in Persian prose;
- do not put a space before punctuation and use one space after it;
- avoid em/en dashes (`—` and `–`) in Persian prose; use a comma, semicolon, parentheses or a new sentence;
- check هکسره: «کتابِ من» is ezafe, while «این کتابه» is colloquial «این کتاب است». In this professional document, write the formal form «این کتاب است»;
- use Persian digits in Persian prose and tables unless the value is a URL, code, version, identifier or other exact Latin source value;
- keep one spelling choice consistent for forms such as «آن‌ها» / «آنها» and «خانه‌ی» / «خانهٔ»;
- keep English product terms and their spelling consistent throughout the document.

## Anti-pattern audit

این موارد را به‌صورت خوشه‌ای بررسی کنید، نه با حذف مکانیکی تک‌واژه‌ها. یک «همچنین» مشکل نیست؛ تکرار «همچنین» همراه با «می‌باشد»، مقدمه‌های کلی و جمع‌بندی‌های بی‌محتوا مشکل است.

- «می‌باشد»، «محسوب می‌شود»، «به شمار می‌رود» و «قرار دارد» وقتی «است» کافی است.
- «نقش بسزایی ایفا می‌کند» و «از اهمیت ویژه‌ای برخوردار است» بدون نتیجه قابل‌بررسی.
- «در دنیای امروز»، «در عصر دیجیتال» و «در نهایت می‌توان گفت» به‌عنوان آغاز یا پایان پیش‌فرض.
- سه‌تایی‌های تبلیغاتی یا قابل‌پیش‌بینی مانند «سریع، آسان و مطمئن».
- «از X تا Y» وقتی این دو سر، یک طیف واقعی نمی‌سازند.
- «کارشناسان معتقدند» یا «تحقیقات نشان می‌دهد» بدون نام منبع.
- ترکیب‌های ترجمه‌ای، عبارت‌های نمایشی، Emoji در Heading و تغییر بی‌دلیل واژه‌ها برای پرهیز از تکرار.

بعد از بازنویسی، متن را با این سؤال بخوانید: «اگر یک خواننده ایرانی این بخش را ببیند، آیا آن را متن ماشینی می‌داند؟» پاسخ نباید با حذف Evidence، محدودیت یا جزئیات واقعی حل شود؛ هدف، نوشتن دقیق‌تر است، نه پنهان‌کردن منشأ متن.

## Human editing pass

Before final delivery, remove formulaic or inflated phrasing, vague authority, redundant paragraphs, forced synonym changes, unsupported analysis, and chatbot framing. Apply targeted edits rather than replacing words mechanically. Preserve meaningful human details, unresolved tension, product terminology, exact numbers, source links, and decisions. Natural writing does not require deliberate mistakes or a promise to bypass AI detectors.
