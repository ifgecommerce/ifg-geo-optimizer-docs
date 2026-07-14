---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Getting Started

<div class="lang-switcher">
  <span class="lang-item lang-current"><img src="assets/flags/gb.svg" alt="" class="flag-icon">English</span>
  <a class="lang-item" href="it/"><img src="assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="de/"><img src="assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="fr/"><img src="assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="es/"><img src="assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

This walks through everything from installing the app to publishing your first AI-optimized FAQ.

## 1. Install and open the dashboard

Once installed, IFG GEO Optimizer opens inside your Shopify admin. The dashboard is your home base — it fills in with your store's GEO score and recent activity as you use the app.

## 2. Fill in your policies

Go to **Settings** and enter your return and shipping policy details (return window, who pays return shipping, handling and transit times, destination country). These feed directly into the structured data the app publishes for every product — Shopify's product pages don't expose this information to search engines otherwise, so this step alone measurably improves your audit score.

## 3. Run your first catalog audit

Open **Audit catalog** and click **Rescan catalog**. The app reads your product catalog through Shopify's Admin API and checks each product against nine structured-data fields search engines look for: image, description, brand, SKU, GTIN, price, technical specs, return policy, and shipping policy.

Products under 80/100 show exactly what's missing. Where the app can fix it automatically — usually by deriving technical specs from your existing product options — you'll see a **Fix** button. One click writes the missing schema.org data straight to the product; nothing is guessed or invented for fields the app can't derive safely (a barcode, for instance, is never auto-generated).

On the Free plan, audits cover your first 20 products and don't keep history. Grow and Unlimited cover your whole catalog and save every scan.

## 4. Turn on the theme block

The structured data your audit fixes doesn't show up on your storefront until you activate it. In your theme editor, go to **App embeds** and turn on **GEO Schema**. This is a one-time toggle — after that, every product page automatically includes the JSON-LD your audit generated.

## 5. Check what a bot actually sees

Open **Crawler AI** and pick a product. The app fetches the page exactly the way an AI crawler does — no JavaScript execution, same as GPTBot, ClaudeBot, or PerplexityBot — so you can see precisely what's visible to these engines, including whether your robots.txt is blocking them and whether your structured data is complete in the raw HTML.

## 6. Generate FAQs

On Grow or Unlimited, open **FAQ product**, pick a product, and click **Generate 3 FAQs**. The app writes three question-and-answer pairs from your product's actual title, description, and specs — never invented details. Review each draft, then **Approve & publish** the ones you want live; approved FAQs appear on your product page and are marked up as FAQPage structured data for search engines. Nothing publishes without your review.

## 7. Choose a plan

**Pricing** shows Free, Grow, and Unlimited side by side, with monthly and annual billing. You can switch plans or cancel back to Free at any time, directly from the app — no need to contact support to downgrade.

That's the full loop. Most merchants re-run an audit after adding new products, and check the crawler simulator whenever they update a product description.

[← Back to Help Center](index.html)
