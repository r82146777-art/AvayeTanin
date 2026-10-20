# موتور داخلی ADB — پیشرفت (۲۰۲۶-۱۰-۲۰)

## انجام‌شده
1. ساخت `jemrec-capture.jar` (دایمون shell از fork JemRec / scrcpy audio) — Apache-2.0 با ذکر منبع
2. قرار دادن jar داخل assets برنامه
3. کلاس‌های `internal/AdbIdentity`, `InternalEngine`, UI جفت‌سازی در تنظیمات
4. نسخه 5.0-internal با همان امضای ۴.۲

## گیر فنی این نشست
- کتابخانه `libadb-android` با d8 فعلی (build-tools 34) هنگام dex خطا می‌دهد (NPE روی PairingConnectionCtx)
- بدون libadb، جفت‌سازی واقعی Wireless Debugging و اجرای دایمون از shell ممکن نیست

## مرحله بعد (وقتی ادامه دادی)
1. بیلد Gradle یا d8 جدیدتر برای libadb + BouncyCastle
2. pair/connect روی 127.0.0.1
3. deploy دایمون با `app_process`
4. اتصال CallRecorderCore به پورت دایمون برای ضبط دوطرفه

## استفاده فعلی
- مسیر پایدار ضبط دوطرفه همچنان: Shizuku + نسخه ۴.۸
- ۵.۰-internal زیرساخت موتور داخلی را دارد ولی جفت‌سازی ADB کامل نیست
