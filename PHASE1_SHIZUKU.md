# فاز ۱ — یکپارچه‌سازی Shizuku در آوای طنین

تاریخ: 2026-10-20
نسخه: 4.6-shizuku (versionCode 10)

## انجام‌شده
- اضافه شدن کتابخانه‌های Shizuku API / Provider / AIDL / Shared
- کلاس `ShizukuHelper` برای تشخیص نصب، اجرا، مجوز
- Provider در AndroidManifest
- UI فارسی در تنظیمات ضبط مکالمه:
  - تیک «موتور سیستم Shizuku»
  - وضعیت Shizuku
  - اعطای مجوز / باز کردن / راهنمای Wireless Debugging
- امضا با همان keystore نسخه ۴.۲

## هنوز انجام نشده (فاز ۲)
- UserService با هویت shell
- AudioRecord روی VOICE_CALL / UPLINK / DOWNLINK
- یا اتصال scrcpy-server برای کپچر صوتی تماس

## نیاز کاربر
1. نصب Shizuku
2. فعال‌سازی با Wireless Debugging
3. اعطای مجوز به آوای طنین از داخل برنامه

تا پایان فاز ۲، ضبط دوطرفه واقعی هنوز به موتور shell وابسته است.
