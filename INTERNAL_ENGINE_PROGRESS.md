# موتور داخلی — پیشرفت v5.1 (۲۰۲۶-۱۰-۲۰)

## انجام‌شده در این مرحله
1. رفع مشکل d8 با build-tools 35 → libadb-android dex شد
2. BouncyCastle برای گواهی ADB (AdbIdentity کامل)
3. InternalAdbManager با AbsAdbConnectionManager
4. pair / connect / deployDaemon واقعی
5. UI راه‌اندازی یک‌مرحله‌ای (پورت جفت‌سازی + کد + پورت اتصال)
6. InternalCaptureClient برای دریافت استریم از دایمون
7. CallRecorderCore: اولویت موتور داخلی قبل از Shizuku
8. jemrec-capture.jar در assets

## امضا
همان SHA1 نسخه ۴.۲: 15:1F:4F:26:...

## تست روی گوشی
1. Developer options + USB debugging + Wireless debugging
2. Pair device with pairing code → پورت و کد
3. همان صفحه IP & port → پورت اتصال
4. در آوای طنین: راه‌اندازی موتور داخلی
5. تماس آزمایشی

## نکات
- بعد از ریستارت گوشی ممکن است Wireless debugging و اتصال مجدد لازم شود
- اگر دایمون روی OEM خاص صدا ندهد، لاگ `/data/local/tmp/avayetanin-capture.log`
- مسیر Shizuku (۴.۸) همچنان به‌عنوان پشتیبان فعال است
