# 🔐 SOC Tier 1 – Basic Website Security Assessment  
Target: xxxxxxxxxxxxx  
IP: xxxxxxxxxxxxx  
Date: xxxxxxxxxxxxx  
Role: SOC Analyst – Trainee  

---

## 🧭 1. Purpose of the Assessment  
This assessment was completed as part of my SOC Tier 1 training to practice basic website security checks and learn how to identify common risks using simple tools.

---

## 🏗 2. Infrastructure & Hosting Review  
Tool Used: *IP Lookup / CDN Checker*

- The website is hosted through a CDN provider: xxxxxxxxxxxx  
- Multiple IP addresses were detected within the same network range:  
  - xxxxxxxxx  
  - xxxxxxxxx  
  - xxxxxxxxx  
  - xxxxxxxxx  

🔎 Summary:  
Standard setup for websites hosted on managed platforms.

---

## 🌐 3. DNS Overview  
Tool Used: *DNS Lookup (A / CNAME Records)*

- No custom DNS records found.  
- Domain relies entirely on the hosting platform’s default DNS settings.  
- Common for template‑based or beginner‑level websites.

🔎 Summary:  
DNS configuration is minimal and fully controlled by the provider.

---

## 🛡 4. Security Headers Check  
Tool Used: *HTTP Header Analyzer*

Missing security headers:

- Content-Security-Policy  
- X-Frame-Options  
- X-Content-Type-Options  
- Referrer-Policy  
- Permissions-Policy  

🔎 Summary:  
These headers help protect against XSS, clickjacking, and data exposure. They can be added later as the site grows.

---

## 🔒 5. TLS/SSL Certificate Review  
Tool Used: *SSL/TLS Checker*

- Certificate Status: Valid  
- Certificate Type: Domain Validation (Wildcard)  
- Algorithm: RSA 2048 bits / SHA256  
- Supported Protocols: TLS 1.2 / TLS 1.3  
- HSTS: Not enabled  
- Expiration Date: xxxxxxxxxxxx

🔎 Summary:  
The certificate is secure, but enabling HSTS would strengthen HTTPS protection.

---

## 🍪 6. Cookies & Exposure Review  
Tool Used: *Browser Developer Tools / Cookie Inspector*

- Platform‑generated cookies detected.  
- Some cookies include general visitor information (e.g., region, city).  
- No visible privacy policy found.

🔎 Summary:  
Data collection is minimal, but adding a privacy policy is recommended.

---

## 📊 7. Risk Summary
| Category | Level |
|---------|--------|
| Infrastructure | Low |
| Security Headers | Medium |
| TLS | Medium |
| Exposure | Medium |
| Overall | Medium Risk |
