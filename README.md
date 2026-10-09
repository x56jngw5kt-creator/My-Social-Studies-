SPRIX Chemistry — Self-contained interactive version

- All core images (SPRIX wordmark, ministry logo, Kimchi, Nitcho) are embedded as data URIs in app.js.
- 26 lesson-specific interactive experiments.
- 26 embedded MP4 micro-explanations; no external video paths.
- 25 independent MCQs for every lesson (650 lesson questions).
- Final review pool of exactly 1000 MCQs; used review questions are stored locally and removed from future review sessions on the same device.
- Virtual lab with all 118 chemical elements, tools, and an equation-balancing checker for common educational equations.
- Arabic speech uses the browser/device speech synthesis engine.
- GitHub Pages ready: upload index.html, app.js and style.css.


## Gemini integration (Ask Kimchi)
- `app.js` calls Gemini API from the browser in Ask Kimchi.
- Paste your key into `GEMINI_API_KEY` in `app.js` before publishing. The key is public on GitHub Pages; monitor quota and rotate it if exposed.
- `chemistry-book-chunks.json` contains extracted text chunks from Chemistry-Ar-EB-part1.pdf and is searched locally to provide relevant textbook context.
- Upload `index.html`, `platform.html`, `app.js`, `style.css`, and `chemistry-book-chunks.json` together to the same Pages root.


## إعداد كيمتشي عبر Groq (بديل مجاني محدود)
- افتح app.js وابحث عن PASTE_YOUR_GROQ_API_KEY_HERE وضع مفتاح Groq الخاص بك محليًا. لا ترسل المفتاح لأي شخص.
- النموذج المستخدم: openai/gpt-oss-120b. الاستخدام المجاني له حدود وقد تتغير.
- GitHub Pages موقع عام؛ المفتاح داخل JavaScript سيكون مرئيًا للزوار. للحماية الفعلية استخدم خادمًا وسيطًا وخزّن المفتاح كمتغير بيئة.
- لم يتم اختبار اتصال حي بمفتاح حقيقي في هذه الحزمة.


## إضافة الفصول الثالث والرابع
- تمت إضافة 26 درسًا من كتاب الكيمياء الجزء الثاني (11 درسًا غير عضويًا و15 درسًا عضويًا).
- لكل درس 25 سؤال اختيار من متعدد.
- تمت إضافة بنوك: كتاب التقييمات الجزء الأول، مراجعة الجزء الثاني (1000 سؤال)، والمستوى الرفيع (250 سؤالًا).
- لم تُعدّل أسطر إعدادات Groq أو دالة askKimchi عمدًا.
- فيديوهات الدروس المضافة هنا شرح مرئي تفاعلي مع قراءة صوتية، وليست تسجيلات محاضرات مصورة.
