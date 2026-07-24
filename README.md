<div align="center">

# TextHuman Admin Dashboard
### Operations interface for the TextHuman platform

![HTML](https://img.shields.io/badge/HTML5-Interface-e34f26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Admin_Logic-f7df1e?style=for-the-badge&logo=javascript&logoColor=111)
![Cloudflare](https://img.shields.io/badge/Cloudflare-Protected_API-f38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-Server--side-3ecf8e?style=for-the-badge&logo=supabase&logoColor=white)

</div>

---

## Overview
Portfolio-safe snapshot of the administrative client used to centralize TextHuman operations while keeping privileged access behind a secured Cloudflare Worker.

## Capabilities
- Usage and revenue summaries
- User and subscription management
- Premium activation and revocation
- Account limit restoration
- Mercado Pago transaction review
- Discount-code management
- Cleanup logs and operational tools

## Secure architecture
```text
Admin browser → protected Cloudflare Worker → Supabase / PostgreSQL
```
The client contains no production service-role credential. Secrets remain in Cloudflare environment variables and privileged actions run server-side.

## Technology
HTML5 · CSS3 · Vanilla JavaScript · Cloudflare Workers API · Supabase · Mercado Pago

## Repository boundary
The current private operations file, real secret values, user records and payment details must never be committed. This repository demonstrates interface and product-development work only.

## Local preview
```bash
git clone https://github.com/abrilvillita/TextHuman-Admin-Dashboard.git
cd TextHuman-Admin-Dashboard
```
Open `index.html`. Connected actions require authorized production configuration.

## Media safety
Only sanitized screenshots or demo accounts belong here. Real emails, transactions and private analytics must be excluded.

---
<div align="center">Part of the [TextHuman](https://humanizatexto.com) ecosystem.</div>
