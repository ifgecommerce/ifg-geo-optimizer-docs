---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Privacy Policy

<div class="lang-switcher">
  <span class="lang-item lang-current"><img src="assets/flags/gb.svg" alt="" class="flag-icon">English</span>
  <a class="lang-item" href="it/"><img src="assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="de/"><img src="assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="fr/"><img src="assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="es/"><img src="assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

**IFG GEO Optimizer** — a Shopify app for Generative Engine Optimization
Last updated: July 2026

## 1. Data Controller

The data controller for personal data processed through **IFG GEO Optimizer** is:

**IFG eCommerce**
Based in Rome, Italy
Email: [ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

## 2. What We Collect

- **Merchant account data (via Shopify OAuth)**: your store domain, an API access token, and the email address on your Shopify account.
- **Catalog data (read-only)**: product titles, descriptions, vendor, prices, options, and technical specifications — used to run audits, simulate crawler behavior, score content extractability, and draft FAQs.
- **Store configuration**: your active plan, the return and shipping policy details you enter in Settings, and any FAQ drafts or approvals you create.
- **Technical data**: request timestamps, internal record identifiers, and system logs.

> The app never requests or receives end-customer data — no names, emails, addresses, or orders. The only Shopify permissions requested are `read_products` and `write_products`.

## 3. Why We Process It, and Under What Legal Basis

We process this data to provide the service you installed the app for — under Art. 6(1)(b) GDPR, performance of a contract: analyzing and improving your catalog's visibility on generative search engines (ChatGPT, Perplexity, Gemini, Google AI Overviews), including drafting FAQs when you explicitly ask for them.

## 4. How We Collect It

Account data is collected once, through Shopify's OAuth flow, when you install the app. Catalog data is read through Shopify's Admin API only when you trigger an action — a scan, a simulation, or a FAQ generation — from the app's dashboard. Nothing runs in the background without you asking for it.

## 5. Who We Share It With

- **Google Firebase / Cloud Firestore** — stores your store configuration, sessions, and FAQ drafts. Google LLC (USA) participates in the EU-US Data Privacy Framework. Data is stored in the europe-west1 region (Belgium).
- **Anthropic PBC (USA)** — provides the language model (Claude) used to draft FAQ suggestions, only when you explicitly request a generation. It receives only the product attributes you've already entered — title, description, vendor, specs — never customer data. See Anthropic's own privacy policy and commercial terms for how they handle that data.
- **Shopify Inc.** — the platform itself, and the source of the Admin API the app uses.

We don't sell data, and we don't use it for marketing or behavioral profiling.

## 6. How Long We Keep It

- **Session tokens**: managed by Shopify's offline-token lifecycle, rotated automatically.
- **Configuration, audits, and FAQ drafts**: kept for as long as the app is installed. Uninstalling triggers Shopify's `shop/redact` webhook, which deletes your store's configuration and sessions entirely.
- **Technical logs**: retained under Google Cloud's standard logging retention.

## 7. Your Rights

Under Articles 15–22 GDPR, you can request access to your data, correction of inaccurate data, or deletion — the simplest way is to uninstall the app — or object to processing. You can also lodge a complaint with your local data protection authority. Since the app never processes end-customer data, the `customers/data_request` and `customers/redact` compliance webhooks respond confirming there's nothing to export or delete.

## 8. Security

All traffic runs over HTTPS/TLS 1.2+. Shopify authentication tokens are never exposed to the browser. Every webhook is verified with a constant-time HMAC SHA-256 check before it's processed. The database is reachable only from the backend, authenticated via the hosting platform's own service identity — there are no static credentials in the code, and direct client access is denied by the database's own security rules. Data is encrypted at rest and in transit.

## 9. Changes

We may update this policy from time to time. Material changes will be reflected here, with the date at the top kept current.

---

**Questions about your data?**
[ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

[← Back to Help Center](index.html)
