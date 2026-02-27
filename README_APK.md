# Cavo – استخراج APK من GitHub (من غير كمبيوتر)

بما إن الريبو **Private** ومش عايز Android SDK على الموبايل، أسهل حل إن GitHub يبني الـ APK لك.

## 1) ارفع التغييرات دي للريبو
اتأكد إن الملف ده موجود:
- `.github/workflows/android-apk.yml`

وإن اللوجو موجود هنا:
- `resources/icon.png`
- `resources/splash.png`

## 2) شغّل الـ Workflow
1. ادخل الريبو على GitHub
2. افتح تبويب **Actions**
3. هتلاقي Workflow باسم: **Build Android APK (Cavo)**
4. دوس **Run workflow**

## 3) حمّل الـ APK
بعد ما الـ build يخلص:
- افتح نفس الـ run
- انزل تحت عند **Artifacts**
- حمّل: **Cavo-debug-apk**

هتلاقي جوّاه ملف:
- `app-debug.apk`

## ملاحظات
- لو عايز نسخة Release موقعة (Signed) قولّي، ونعمل Workflow تاني مع Keystore.
