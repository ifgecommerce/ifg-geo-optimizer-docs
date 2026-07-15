---
title: IFG GEO Optimizer
description: Documentatie, veelgestelde vragen en juridische pagina's voor de Shopify-app IFG GEO Optimizer.
lang: nl
---

# Privacybeleid

<div class="lang-switcher">
{% include lang-switcher.html current="nl" slug="privacy" %}
</div>

**IFG GEO Optimizer** — een Shopify-app voor Generative Engine Optimization
Laatst bijgewerkt: juli 2026

## 1. Verwerkingsverantwoordelijke

De verwerkingsverantwoordelijke voor persoonsgegevens die worden verwerkt via **IFG GEO Optimizer** is:

**IFG eCommerce** — gevestigd in Rome, Italië
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Wat we verzamelen

- **Accountgegevens van de winkelier (via Shopify OAuth)**: je winkeldomein, een API-toegangstoken en het e-mailadres dat aan je Shopify-account is gekoppeld.
- **Catalogusgegevens (alleen-lezen)**: producttitels, beschrijvingen, leverancier, prijzen, opties en technische specificaties — gebruikt om audits uit te voeren, crawlergedrag te simuleren, content-extraheerbaarheid te scoren en FAQ's of herschreven beschrijvingen op te stellen.
- **Winkelconfiguratie**: je actieve pakket, de details van je retour- en verzendbeleid en bedrijfsgegevens die je invoert in Instellingen, opgeslagen audits, FAQ- en content-herschrijfconcepten, en de prompts die je kiest om te volgen voor AI-visibility.
- **Supportchatberichten**: de tekst die je uitwisselt met de AI-assistent in de app, inclusief het transcript dat naar ons wordt doorgestuurd als je expliciet vraagt om met een mens te spreken.
- **Anonieme storefront-gegevens (Web Pixel, Grow/Unlimited)**: wanneer een bezoeker op een productpagina terechtkomt via een herkende AI-engine (ChatGPT, Perplexity, Claude, Gemini, Copilot), registreren we de engine, de pagina-URL en een tijdstempel — alleen als de bezoeker al toestemming heeft gegeven voor analytics via de cookiebanner van je winkel. Er wordt geen bezoekersidentificatie, cookie of sessiegegeven verzameld.
- **Technische gegevens**: tijdstempels van verzoeken, interne recordidentificatoren en systeemlogs.

> De app **vraagt of ontvangt nooit persoonsgegevens van eindklanten** — geen namen, e-mailadressen, adressen of bestellingen. De gevraagde Shopify-permissies zijn `read_products`, `write_products` (catalogus en gestructureerde data), `read_themes` (controleren of de thema-embed actief is) en `write_pixels` (het activeren van de hierboven beschreven anonieme verkeerspixel).

## 3. Waarom we het verwerken, en op welke rechtsgrond

We verwerken deze gegevens om de dienst te leveren waarvoor je de app hebt geïnstalleerd — op grond van Art. 6(1)(b) AVG, uitvoering van een overeenkomst: het analyseren en verbeteren van de zichtbaarheid van je catalogus op generatieve zoekmachines, inclusief AI-ondersteund opstellen van FAQ's en content herschrijven, de supportchat in de app, wekelijkse AI-visibility-tracking op prompts die je zelf kiest, en anonieme meting van AI-doorverwijzingsverkeer — allemaal ofwel geïnitieerd door de winkelier, of, voor de verkeerspixel, afhankelijk van toestemming op je storefront.

## 4. Hoe we het verzamelen

Accountgegevens worden eenmalig verzameld, via de OAuth-flow van Shopify, bij installatie. Catalogusgegevens worden alleen gelezen via de Admin API van Shopify wanneer je een actie vanuit het dashboard start. De verkeerspixel draait op je storefront en rapporteert gebeurtenissen pas na toestemming; er gebeurt niets anders op de achtergrond zonder dat jij daarom vraagt.

## 5. Met wie we het delen

- **Google Firebase / Cloud Firestore** — bewaart je configuratie, sessies en concepten. Google LLC (VS) neemt deel aan het EU-VS Data Privacy Framework. Gegevens worden opgeslagen in de regio europe-west1 (België).
- **Anthropic PBC (VS)** — levert het Claude-model dat wordt gebruikt voor het opstellen van FAQ's, content herschrijven en de supportchat in de app, alleen op jouw expliciete actie. Ontvangt alleen de productattributen of chattekst die je zelf verstrekt — nooit klantgegevens.
- **OpenAI, Inc. (VS)** en **Perplexity AI, Inc. (VS)** — uitsluitend gebruikt voor de wekelijkse AI-visibility-tracking op de prompts die je expliciet kiest om te volgen. Ontvangen alleen de gevolgde prompttekst — nooit klantgegevens.
- **Google LLC (VS)** — levert het Gemini-model, op dezelfde manier gebruikt als OpenAI/Perplexity hierboven voor visibility-tracking (een apart gebruik dan Firebase/Firestore, dat alleen opslag betreft).
- **Resend, Inc. (VS)** — stuurt ons een melding, met de winkelnaam en het transcript van de supportchat, alleen wanneer je expliciet vraagt om met een mens te spreken in de supportchat.
- **Shopify Inc.** — het platform zelf, en de bron van de Admin API en de Web Pixel-infrastructuur die de app gebruikt.

We verkopen geen gegevens en gebruiken ze niet voor marketing of gedragsprofilering.

## 6. Hoe lang we het bewaren

- **Sessietokens**: beheerd via de levenscyclus van Shopify's offline tokens, automatisch vernieuwd.
- **Configuratie, audits, concepten en verkeersgebeurtenissen**: bewaard zolang de app geïnstalleerd is. Deïnstalleren activeert de `shop/redact`-webhook van Shopify, die de configuratie en sessies van je winkel volledig verwijdert.
- **Technische logs**: bewaard volgens het standaard logbewaarbeleid van Google Cloud.

## 7. Jouw rechten

Op grond van Artikelen 15–22 AVG kun je inzage vragen in je gegevens, correctie van onjuiste gegevens, of verwijdering — de eenvoudigste manier is de app te deïnstalleren — of bezwaar maken tegen verwerking. Je kunt ook een klacht indienen bij je lokale toezichthoudende autoriteit voor gegevensbescherming. Omdat de app nooit persoonsgegevens van eindklanten verwerkt, bevestigen de compliance-webhooks `customers/data_request` en `customers/redact` dat er niets te exporteren of te verwijderen is.

## 8. Beveiliging

Al het verkeer loopt via HTTPS/TLS 1.2+. Shopify-authenticatietokens worden nooit blootgesteld aan de browser. Elke webhook wordt geverifieerd met een constant-time HMAC SHA-256-controle voordat deze wordt verwerkt. De database is alleen bereikbaar vanuit de backend, geauthenticeerd via de eigen service-identiteit van het hostingplatform — er staan geen statische inloggegevens in de code, en directe clienttoegang wordt geweigerd door de eigen beveiligingsregels van de database. Gegevens worden zowel in rust als tijdens verzending versleuteld.

## 9. Wijzigingen

We kunnen dit beleid van tijd tot tijd bijwerken. Materiële wijzigingen worden hier weergegeven, met de datum bovenaan actueel gehouden.

---

**Vragen over je gegevens?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Terug naar Helpcentrum](index.html)
