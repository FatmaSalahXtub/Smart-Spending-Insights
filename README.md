# مصروفي · Masroufi

دفتر مصاريف الطالب التونسي — React + Express.
Gestion des dépenses de l'étudiant tunisien — Student expense tracker.

## التشغيل · Lancement · Run

```bash
npm install
cp .env.example .env      # (Windows: copy .env.example .env)
npm run dev
```

ثم افتح الرابط الذي يظهر في الطرفية (غالبًا http://localhost:3000).
مفتاح `GEMINI_API_KEY` في `.env` اختياري: بدونه تعمل ميزات الذكاء الاصطناعي بقواعد بسيطة.

حساب التجربة / Compte démo : `etudiant@masroufi.tn` / `password123`
يمكنك تغيير الاسم من صفحة **الملف الشخصي (Profile)**.

## ما الجديد
- **3 لغات**: العربية (RTL) · Français · English، يبدّلها الزر في أعلى الصفحة وتُحفظ في المتصفح.
- **الدينار التونسي (DT / د.ت)** عملة افتراضية. (التخزين الداخلي بالروبية ثم يُحوَّل بسعر الصرف الحي.)
- **ألوان جديدة**: أزرق سيدي بوسعيد + أحمر العلم + نقش «الخاتم» الهندسي.
- **خطوط**: Cairo للعربية و Plus Jakarta Sans للّاتينية (تُحمَّل من Google Fonts).
- وسائل دفع وأمثلة تونسية (D17، فلوسي، لواج، أوريدو…).

## إضافة أو تعديل ترجمة
كل النصوص في `src/lib/translations.ts` على شكل: `'English text': ['عربي', 'Français']`.
المحوّل `src/lib/i18n.ts` يترجم الصفحة تلقائيًا دون تغيير مكوّنات React.
