# Results-2026 — مدرسة أبو القاسم الزهراوي

نظام بطاقة الإنجاز الأكاديمي الذكية — الدور الأول ٢٠٢٥/٢٠٢٦

---

## 🗂️ هيكل المشروع

```
Results-2026/
├── index.html       ← الصفحة الرئيسية (لا تعدّلها)
├── grades.json      ← بيانات الدرجات ← هنا تضيف الشعب
├── assets/
│   └── logo.png     ← شعار المدرسة
└── README.md
```

---

## ➕ إضافة شعبة جديدة

افتح `grades.json` وأضف الشعبة داخل `"classes"`:

```json
{
  "classes": {
    "5-1": { "grade": "الخامس", "size": 40, "students": [...] },
    "5-2": { "grade": "الخامس", "size": 41, "students": [...] }
  }
}
```

كل طالب يكون بهذا الشكل:
```json
{
  "name": "اسم الطالب",
  "civil_id": "12345678",
  "class_name": "5-2",
  "grade": "الخامس",
  "subjects": {
    "التربية الاسلامية": { "level": "أ", "score": 95 },
    "اللغة العربية":     { "level": "أ", "score": 98 }
  },
  "total": 930,
  "max_total": 1000,
  "percentage": 93.0,
  "class_rank": 3,
  "grade_rank": 3,
  "_class_size": 41
}
```

---

## 🚀 رفع المشروع على GitHub Pages

```bash
# 1. استنسخ الريبو
git clone https://github.com/sc1561/Results-2026.git
cd Results-2026

# 2. انسخ ملفات المشروع هنا ثم:
git add .
git commit -m "initial setup"
git push origin main

# 3. فعّل GitHub Pages:
#    Settings → Pages → Source → main → / (root)
```

سيصبح الموقع متاحاً على:
```
https://sc1561.github.io/Results-2026/
```

---

## 📌 ملاحظات

- البحث يتم بالرقم المدني فقط
- المشاركة تتم كصورة PNG عبر واتساب
- يدعم إضافة شعب جديدة بدون تعديل `index.html`

---

⚡ برمجة وتصميم **أستاذ أحمد الضامري**
