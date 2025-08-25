# Security — احراز هویت و مجوزدهی

## OAuth2 / OIDC / JWT
- پشتیبانی از **Client Credentials**، **Authorization Code + PKCE** برای اپلیکیشن‌های محرمانه/عمومی.
- **JWT** امضا شده (JWS) با **Scopes** برای تفکیک دسترسی‌ها.
- امکان **Token Exchange (RFC 8693)** برای تعویض توکن بین دامنه‌ها/کلاینت‌ها.

## mTLS (Mutual TLS)
- الزام ارائه‌ی **Client Certificate** در سطح Gateway برای کانال‌های حساس (پرداخت/انتقال وجه).
- جداسازی سطوح اعتماد با **Truststore**‌های مجزا برای شرکا.

## Scopes & Consent
- تعریف **Scope**‌ها در سطح API/Resource.
- ثبت **Consent** کاربر نهایی (در صورت نیاز به الگوی Open Banking) در IdP/Consent Store.

## Threat Protection
- **DoS/DDoS Throttling**، IP Allow/Deny، CORS، Data Masking، XML/JSON threat protection.
- سیاست‌های **PII Redaction** در لاگ‌ها.

## Key Managers
- اتصال به **WSO2 IS** یا IdPهای دیگر (Keycloak/ADFS/…).
- چند-Key Manager برای جداسازی B2B/B2C/Internal.
