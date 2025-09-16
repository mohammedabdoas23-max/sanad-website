# منصة سند — موقع متعدد الصفحات

هذا موقع ثابت (Static) بثلاث صفحات رئيسية:
- index.html (الرئيسية)
- services.html (الخدمات والباقات)
- contact.html (التواصل وبيانات التحويل اليدوي)

## النشر على GitHub Pages
1) أنشئ مستودع جديد في GitHub باسم: `sanad-website`
2) ارفع جميع الملفات كما هي (في الجذر).
3) من Settings → Pages:
   - اختر Branch: `main`
   - اختر Folder: `/ (root)`
   - Save
4) الرابط سيكون: `https://USERNAME.github.io/sanad-website` (بدّل USERNAME باسم حسابك في GitHub).

### أوامر Git (اختياري)
```bash
git init
git add .
git commit -m "Initial Sanad website"
git branch -M main
git remote add origin https://github.com/USERNAME/sanad-website.git
git push -u origin main
```
