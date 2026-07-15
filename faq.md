---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Frequently Asked Questions

<div class="lang-switcher">
{% include lang-switcher.html current="en" slug="faq" %}
</div>

**What's the difference between GEO and SEO?**
Traditional SEO optimizes for search engines that rank and list links. GEO (Generative Engine Optimization) optimizes for AI systems that read your content and generate an answer or a recommendation directly — ChatGPT, Perplexity, Gemini, Claude, and Google AI Overviews. The two overlap, but GEO cares about things classic SEO tools don't check: whether your product page has complete structured data, whether an AI crawler can actually read your content without executing JavaScript, and whether your copy is written in a way that's easy to quote and cite.

**Does the app ever touch my customers' data?**
No personal customer data. The app's Shopify permissions are `read_products`, `write_products`, `read_themes`, and `write_pixels` — reading and improving your catalog, checking the theme embed is active, and activating an anonymous storefront-traffic pixel (see below). It never requests orders or customer records. See the [Privacy Policy](privacy.html) for the full breakdown.

**What is the AI referral traffic pixel, and does it track my customers?**
On Grow and Unlimited, a small Web Pixel detects when a storefront visit arrives from a known AI engine (via the browser referrer) and reports the engine, the page, and a timestamp — nothing that identifies the visitor, no cookies, no session data. It only runs if the visitor has already given analytics consent through your store's cookie banner (Shopify's Customer Privacy API). It's used to show a Dashboard tile ("AI referral traffic, last 7 days") — the counterpart to the Visibility AI tracking, which tells you if you're mentioned but not whether that mention sent anyone.

**What does the "Fix" button on the catalog audit actually change?**
It writes missing schema.org structured data to a product metafield — things like technical specifications derived from your existing product options. It never touches your product title, description, images, or price, and it never invents data it can't verify: a missing barcode, for example, stays missing rather than being guessed.

**Are the FAQ answers and rewritten descriptions made up by AI, or based on my actual product?**
The model only sees the product data you already have — title, description, vendor, and technical specs — and is explicitly instructed not to add anything not present in that data. You review every FAQ or rewritten description before it publishes; nothing goes live automatically.

**What happens to my data if I uninstall the app?**
Your store configuration, saved audits, FAQ and content-rewrite drafts, visibility prompts, and AI referral traffic events are deleted automatically when Shopify notifies us of the uninstall. The app doesn't hold onto anything after you leave.

**Can I cancel or downgrade without contacting support?**
Yes. Go to **Pricing** inside the app and switch to Free at any time — it takes effect immediately, no email required.

## Plan limits

| Feature | Free | Grow | Unlimited |
|---|---|---|---|
| Catalog audit | First 20 products, one-time, no history | Full catalog + history | Full catalog + history |
| Crawler simulator | 20/month | 300/month | 1,000/month |
| Competitor comparison | 10/month | 50/month | 150/month |
| FAQ generation | Not included | 500/month | 500/month |
| Content rewrite | Not included | 300/month | 300/month |
| Visibility AI (tracked prompts) | Not included | 5 prompts | 15 prompts |
| AI referral traffic pixel | Not included | Included | Included |
| AI support chat | 1,000 messages/month | 1,000 messages/month | 1,000 messages/month |
| Interface languages | All 30 | All 30 | All 30 |

Monthly pricing: Free $0, Grow $9.99, Unlimited $19.99. Annual billing on Grow/Unlimited is roughly two months free compared to paying monthly.

**Why does the Free plan only cover 20 products?**
It's meant to let you see real results on your own catalog before committing to a paid plan. Grow and Unlimited remove that cap and keep a full history of past audits.

**Is there really a cap on FAQ generation even on Unlimited?**
Yes — 500 generations a month, deliberately, even on the top plan. This keeps the feature sustainable at the current price; if you're a high-volume catalog that needs more, get in touch and we'll work something out.

**Why is the AI support chat the same on every plan?**
It's a product decision, not an oversight: assistance is included for everyone, never a paid differentiator. The message cap (1,000/month) exists only as a technical safeguard against abuse, not as a real-world limit — no legitimate use comes close to it.

**I found a bug or something looks wrong. Who do I tell?**
Email [info@ifgecommerce.com](mailto:info@ifgecommerce.com) with what you saw and, if you can, which product or page — that's usually enough to track it down quickly. You can also use the AI support chat inside the app and ask to talk to a human.

[← Back to Help Center](index.html)
