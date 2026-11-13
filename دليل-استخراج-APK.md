# دليل استخراج ملف Android APK لتطبيق: الجديد — بحث الأصناف

## أسرع طريقة بدون Android Studio (عبر GitHub Actions مجانًا)
1. أنشئ مستودعًا (Repository) جديدًا على GitHub.
2. فك ضغط هذا الملف وارفع جميع المجلدات (بما فيها مجلد `.github`) إلى المستودع.
3. ادخل إلى تبويب **Actions** في المستودع واختر **Build Android APK** ثم اضغط **Run workflow**.
4. بعد دقيقتين تقريبًا، ادخل على النتيجة واضغط تحميل **aljadeed-android-apk** للحصول على ملف `app-debug.apk` الجاهز للتثبيت على أندرويد.

## الطريقة الثانية (عبر Android Studio على الكمبيوتر)
1. افتح مجلد `android-webview-apk` من داخل برنامج **Android Studio**.
2. انتظر انتهاء مزامنة Gradle.
3. من القائمة العلوية اختر: `Build > Build Bundle(s) / APK(s) > Build APK(s)`.
4. ستجد ملف الـ APK الناتج في: `android-webview-apk/app/build/outputs/apk/debug/app-debug.apk`.

## ملاحظات مهمة داخل المشروع المُصدّر
- تم تفعيل `domStorageEnabled` لحفظ تعديلات الأسعار وقاعدة البيانات المستوردة محليًا بدون إنترنت.
- تم تفعيل صلاحية الكاميرا ومعالج اختيار الصور والملفات (`onShowFileChooser`) لعمل مسح الباركود واستيراد ملفات PDF/Excel.
- تم تضمين معالج تصدير النسخة الاحتياطية JSON لمشاركتها أو حفظها على الهاتف.
