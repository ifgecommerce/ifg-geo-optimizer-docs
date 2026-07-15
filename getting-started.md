---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Getting Started

<div class="lang-switcher">
{% include lang-switcher.html current="en" slug="getting-started" %}
</div>

IFG GEO Optimizer has nine areas, all reachable from the top navigation once setup is done: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings**, and **Support**. This guide walks through all of them, in the order most merchants use them.

## 1. Install and complete the setup wizard

On first open, a short guided setup (about 2 minutes) collects the basics: interface language, your return and shipping policy details, your company information, and — the one step that actually matters technically — activating the **GEO Schema** app embed in your theme editor. Nothing the app does afterwards reaches your storefront until this embed is turned on, so it's worth not skipping. You can always change any of these answers later from **Settings**.

## 2. Dashboard

Your home base. It shows your current GEO score (from your last audit), a **Readiness Matrix** with eight at-a-glance signals — content extractability, Organization schema, `llms.txt`, `agents.md`, crawler access, MCP readiness, Link Coach connectivity, and AI referral traffic — plus a prioritized "fix this first" list and your plan's usage counters (FAQ generations, catalog size). Everything here links straight to the page where you can act on it.

## 3. Audit catalog

Click **Rescan catalog** to check every product against nine structured-data fields search engines look for: image, description, brand, SKU, GTIN, price, technical specs, return policy, and shipping policy. Products under 80/100 show exactly what's missing.

- **One-click fix**: where the app can safely derive the missing data (usually technical specs from your existing product options), you'll see a **Fix** button that writes it straight to the product's structured data. Nothing is guessed for fields the app can't verify — a missing barcode, for instance, stays missing rather than being invented.
- **Content chunking score**: alongside the structured-data check, every product gets a separate extractability score — not "is the field present" but "can an AI/RAG system actually pull a clean fact out of this description." Thin, adjective-heavy copy scores lower even with perfect schema.org markup.
- **`llms.txt`**: generates a real, standards-compliant `llms.txt` file summarizing your catalog for AI systems, served at your store's true root (`/llms.txt`), not buried under an app proxy path where crawlers won't find it.
- **`agents.md`**: generates a file describing your store to autonomous shopping agents — variants, search, checkout — built only from real data your store already exposes, nothing invented.
- **Organization schema**: publishes your company details (legal name, VAT/tax ID, address) as structured data, so AI engines can verify you're a real, accountable business before recommending you.

On Free, audits cover your first 20 products, one-time, with no history kept. Grow and Unlimited scan your whole catalog and keep every past scan for trend comparison.

## 4. Crawler AI

Pick a product and the app fetches its page exactly the way an AI crawler does — no JavaScript execution, same as GPTBot, ClaudeBot, or PerplexityBot — so you see precisely what's visible to these engines: whether your `robots.txt` blocks them (checked per-bot, not just a generic allow/deny), and whether your structured data actually survives in the raw HTML these bots read.

**Competitor comparison** (its own tab from this page): paste a competitor's product URL and get the same GEO signals compared side by side with yours — same difference-in-kind you'd get from a manual audit, without needing to sign up for the competitor's own tools.

## 5. FAQ product

On Grow or Unlimited, pick a product and click **Generate FAQs** for three to five question-and-answer pairs drafted only from that product's real title, description, vendor, and specs — the model is explicitly instructed never to add a detail that isn't already in your data. Review every draft; nothing publishes without your explicit **Approve**. Approved FAQs appear on the live product page and are marked up as `FAQPage` structured data, so they're both human-readable and machine-citable.

**Content rewrite** (its own tab from this page): the app can rewrite a product description to be denser in verifiable facts and easier for a generative engine to quote — you always see a before/after comparison and approve before anything is written back to the product.

## 6. Link Coach

Analyzes how well your products are connected to each other through shared collections, vendors, and tags — internal linking is a signal AI systems use to understand what your catalog covers as a whole, not just one page at a time. Shows orphaned products with no meaningful connections and explainable suggestions to fix that.

## 7. Visibility AI

Add up to a handful of prompts you'd realistically expect a customer to ask an AI assistant (limit depends on your plan — see Pricing below), and every week the app checks whether Claude, ChatGPT, Gemini, and Perplexity mention your store in the answer, tracked over time per engine. On Grow and Unlimited, this also shows how you compare to named competitors on the same prompts.

**AI referral traffic** (Grow and Unlimited): a lightweight, privacy-respecting pixel detects when a storefront visit actually originates from one of these AI engines (via referrer, only after the visitor has given analytics consent through your store's cookie banner) and reports how many such visits you got in the last 7 days — the second half of the loop that visibility tracking alone can't show: not just "are we mentioned," but "is that mention sending anyone."

## 8. Support

An AI chat assistant lives in the app (bottom-right icon) for questions about GEO, your audit results, or how a specific feature works. If it can't help, you can ask to talk to a human and the conversation is forwarded to IFG eCommerce directly.

## 9. Settings

Where you manage the setup-wizard answers (policies, company data, interface language — switch instantly among 30 languages, no reload lag), re-check the theme embed activation, and see your account's Shopify scopes.

## 10. Pricing

**Pricing** shows Free, Grow, and Unlimited side by side, monthly or annual (annual is roughly 2 months free on both paid tiers). You can upgrade, downgrade, or cancel back to Free at any time, directly from the app — no email required. See the [FAQ](faq.html) for exact plan limits.

That's the full loop. Most merchants re-run an audit after adding new products, check the crawler simulator whenever they update a description, and glance at the Dashboard's Readiness Matrix weekly.

[← Back to Help Center](index.html)
