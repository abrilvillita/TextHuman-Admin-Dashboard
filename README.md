# TextHuman Admin Dashboard

Administrative dashboard for managing the TextHuman platform through its secured Cloudflare Worker API.

## Overview

This interface centralizes operational tasks for TextHuman, including:

- Platform usage and revenue statistics
- User and subscription management
- Premium activation and revocation
- Account limit restoration
- Mercado Pago transaction review
- Discount-code management
- Administrative tools and system information

The dashboard does **not** connect directly to the production database. Sensitive
operations are delegated to a private API endpoint, and no production credentials
are included in this repository.

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Cloudflare Workers API
- Supabase (server-side access through the Worker)
- Mercado Pago integration

## Security notes

- Secrets and service-role credentials must remain in Cloudflare environment variables.
- Never commit `.env` files, API keys, admin secrets, or database credentials.
- This repository contains the dashboard client only; access still requires server-side authorization.
- Use a private/local copy for real administrative work.

## Related project

[TextHuman live application](https://humanizatexto.com)

## Status

Active personal project. The public repository documents the interface and
architecture; production configuration is intentionally excluded.
