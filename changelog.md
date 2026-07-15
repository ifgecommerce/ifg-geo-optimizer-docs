---
title: IFG GEO Optimizer
description: Documentation, FAQ, and legal pages for the IFG GEO Optimizer Shopify app.
---

# Changelog

<div class="lang-switcher">
{% include lang-switcher.html current="en" slug="changelog" pages="en,it,de,fr,es" %}
</div>

All changes that reach merchants, newest first. This is technical documentation, kept in 5 languages (English, Italian, German, French, Spanish) rather than all 30 the rest of the Help Center supports.

## July 2026

**AI referral traffic tracking** — Added a Web Pixel (Grow/Unlimited) that detects storefront visits arriving from a recognized AI engine (ChatGPT, Perplexity, Claude, Gemini, Copilot) and reports them on a new Dashboard tile, consent-gated and fully anonymous — the counterpart to Visibility AI tracking: not just "are we mentioned," but "is that mention sending anyone."

**Dashboard and navigation polish** — Added a proper empty state for first-time use, a loading skeleton during page navigation, and a per-bot breakdown on the crawler page showing whether a `robots.txt` rule was matched by name or inherited from the wildcard group.

**Onboarding redesign** — The setup wizard's progress bar became a step-by-step checklist, with a visible confirmation banner on completion instead of an instant, unconfirmed reload.

**Billing and support email** — Support and privacy contact moved to `info@ifgecommerce.com`.

**Internal Link & Entity Graph Coach** — New analysis of how well products connect to each other through shared collections, vendors, and tags, with explainable suggestions and a Dashboard summary.

**Readiness Matrix** — The Dashboard gained a single, at-a-glance panel aggregating every GEO signal the app tracks: content extractability, Organization schema, `llms.txt`, `agents.md`, crawler access, MCP readiness, Link Coach connectivity, and (once shipped) AI referral traffic.

**Content rewrite engine** — Added an AI-assisted tool to rewrite a product description to be denser in verifiable facts and easier for a generative engine to quote, with a mandatory before/after review before anything is written back.

**Competitor comparison** — Paste a competitor's product URL and see the same GEO signals compared side by side with your own product.

**Visibility AI tracking** — Weekly automated checks of whether Claude, ChatGPT, Gemini, and Perplexity mention your store on prompts you choose to monitor, with a trend chart and per-engine breakdown.

**Organization schema and `agents.md`** — Added structured company-identity data (legal name, VAT/tax ID, address) for AI systems verifying a business is real, and a generated `agents.md` file describing the store to autonomous shopping agents.

**Billing** — Merchants can subscribe to Grow or Unlimited, monthly or annual, directly from the Pricing page, and cancel back to Free at any time without contacting support.

**Privacy policy and App Store compliance review** — Published this Help Center and a formal privacy policy; confirmed the app's Shopify permissions and GDPR webhook handling meet App Store requirements ahead of submission.

**AI-assisted FAQ generation** — Generate three to five question-and-answer pairs per product from its existing title, description, and specs, review them, and publish the ones you approve. Published FAQs appear on the product page and as `FAQPage` structured data.

**Content extractability (chunking) score** — The catalog audit now also scores how easy each product's description is for an AI system to extract and quote from — not just whether structured-data fields are present, but whether the writing itself is usable.

**Crawler simulator** — Fetch any product page exactly as an AI crawler sees it — no JavaScript, same as GPTBot, ClaudeBot, and PerplexityBot — including per-bot `robots.txt` checks.

**Catalog audit and one-click fixes** — Launched the core audit: scans your catalog against nine structured-data fields, scores each product, and fixes what it safely can with one click. Also added real `llms.txt` generation, served at your store's true root.

## Earlier

Initial release: embedded app setup, Shopify authentication, and the underlying data infrastructure.

[← Back to Help Center](index.html)
