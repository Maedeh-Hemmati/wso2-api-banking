# Overview — معماری API Banking با WSO2

**هدف:** تبدیل سرویس‌های بانکی (Core/ESB/Microservices) به APIهای استاندارد و قابل مصرف برای شرکای بیرونی/درونی.

## اجزای کلیدی
- **Publisher**: ایجاد/ویرایش API، تعریف ورژن، مستندات، تست، و انتشار.
- **Developer Portal**: آنبورد توسعه‌دهندگان، ساخت Application، گرفتن کلید/توکن، سابسکریپشن.
- **Gateway (WSO2 Gateway یا Choreo Connect)**: اجرای سیاست‌ها، امنیت، مسیریابی، محدودسازی.
- **Key Manager**: صدور/اعتبارسنجی توکن‌ها (OAuth2/JWT)، مدیریت Scope/Consent (با IdP).
- **Analytics**: مانیتورینگ مصرف، خطا، تاخیر، گزارش‌دهی SLA.

## جریان کلی
1. تیم بانک API را در **Publisher** تعریف و منتشر می‌کند.
2. مشتری/فین‌تک در **Dev Portal** ثبت‌نام، **Application** ایجاد و برای API **Subscribe** می‌کند.
3. **Key Manager** توکن صادر می‌کند. **Gateway** احراز هویت/مجوز، Throttling و مسیریابی را انجام می‌دهد.
4. **Analytics** مصرف و سلامت را قابل مشاهده می‌کند.
