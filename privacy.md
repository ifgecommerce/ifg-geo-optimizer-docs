---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Privacy Policy

<div class="lang-switcher">
{% include lang-switcher.html current="en" slug="privacy" %}
</div>

**IFG GEO Optimizer** — a Shopify app for Generative Engine Optimization
Last updated: July 2026

## 1. Data Controller

The data controller for personal data processed through **IFG GEO Optimizer** is:

**IFG eCommerce** — based in Rome, Italy
Email: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. What We Collect

- **Merchant account data (via Shopify OAuth)**: your store domain, an API access token, and the email address on your Shopify account.
- **Catalog data (read-only)**: product titles, descriptions, vendor, prices, options, and technical specifications — used to run audits, simulate crawler behavior, score content extractability, and draft FAQs or rewritten descriptions.
- **Store configuration**: your active plan, the return and shipping policy details and company data you enter in Settings, saved audits, FAQ and content-rewrite drafts, and the prompts you choose to track for AI visibility.
- **Support chat messages**: the text you exchange with the in-app AI assistant, including the transcript forwarded to us if you explicitly ask to speak to a human.
- **Anonymous storefront traffic (Web Pixel, Grow/Unlimited)**: when a visitor arrives at a product page from a recognized AI engine (ChatGPT, Perplexity, Claude, Gemini, Copilot), we record the engine, the page URL, and a timestamp — only if the visitor has already given analytics consent through your store's cookie banner. No visitor identifier, cookie, or session data is collected.
- **Technical data**: request timestamps, internal record identifiers, and system logs.

> The app **never requests or receives personal end-customer data** — no names, emails, addresses, or orders. The Shopify permissions requested are `read_products`, `write_products` (catalog and structured data), `read_themes` (checking the theme embed is active), and `write_pixels` (activating the anonymous traffic pixel above).

## 3. Why We Process It, and Under What Legal Basis

We process this data to provide the service you installed the app for — under Art. 6(1)(b) GDPR, performance of a contract: analyzing and improving your catalog's visibility on generative search engines, including AI-assisted FAQ drafting and content rewriting, the in-app support chat, weekly AI-visibility tracking on prompts you choose, and anonymous AI-referral traffic measurement — all either merchant-initiated or, for the traffic pixel, consent-gated on your storefront.

## 4. How We Collect It

Account data is collected once, through Shopify's OAuth flow, at install. Catalog data is read through Shopify's Admin API only when you trigger an action from the dashboard. The traffic pixel runs on your storefront and reports events only after consent; nothing else runs in the background without you asking for it.

## 5. Who We Share It With

- **Google Firebase / Cloud Firestore** — stores your configuration, sessions, and drafts. Google LLC (USA) participates in the EU-US Data Privacy Framework. Data is stored in the europe-west1 region (Belgium).
- **Anthropic PBC (USA)** — provides the Claude model used for FAQ drafting, content rewriting, and the in-app support chat, only on your explicit action. Receives only the product attributes or chat text you provide — never customer data.
- **OpenAI, Inc. (USA)** and **Perplexity AI, Inc. (USA)** — used exclusively for weekly AI-visibility tracking on the prompts you explicitly choose to monitor. Receive only the tracked prompt text — never customer data.
- **Google LLC (USA)** — provides the Gemini model, used the same way as OpenAI/Perplexity above for visibility tracking (a distinct use from Firebase/Firestore, which is storage only).
- **Resend, Inc. (USA)** — sends us a notification, with the store name and support-chat transcript, only when you explicitly ask to talk to a human in the support chat.
- **Shopify Inc.** — the platform itself, and the source of the Admin API and Web Pixel infrastructure the app uses.

We don't sell data, and we don't use it for marketing or behavioral profiling.

## 6. How Long We Keep It

- **Session tokens**: managed by Shopify's offline-token lifecycle, rotated automatically.
- **Configuration, audits, drafts, and traffic events**: kept for as long as the app is installed. Uninstalling triggers Shopify's `shop/redact` webhook, which deletes your store's configuration and sessions entirely.
- **Technical logs**: retained under Google Cloud's standard logging retention.

## 7. Your Rights

Under Articles 15–22 GDPR, you can request access to your data, correction of inaccurate data, or deletion — the simplest way is to uninstall the app — or object to processing. You can also lodge a complaint with your local data protection authority. Since the app never processes personal end-customer data, the `customers/data_request` and `customers/redact` compliance webhooks respond confirming there's nothing to export or delete.

## 8. Security

All traffic runs over HTTPS/TLS 1.2+. Shopify authentication tokens are never exposed to the browser. Every webhook is verified with a constant-time HMAC SHA-256 check before it's processed. The database is reachable only from the backend, authenticated via the hosting platform's own service identity — there are no static credentials in the code, and direct client access is denied by the database's own security rules. Data is encrypted at rest and in transit.

## 9. Changes

We may update this policy from time to time. Material changes will be reflected here, with the date at the top kept current.

---

**Questions about your data?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Back to Help Center](index.html)
