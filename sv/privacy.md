---
title: IFG GEO Optimizer
description: Dokumentation, FAQ och juridiska sidor för Shopify-appen IFG GEO Optimizer.
lang: sv
---

# Integritetspolicy

<div class="lang-switcher">
{% include lang-switcher.html current="sv" slug="privacy" %}
</div>

**IFG GEO Optimizer** — en Shopify-app för Generative Engine Optimization
Senast uppdaterad: juli 2026

## 1. Personuppgiftsansvarig

Personuppgiftsansvarig för persondata som behandlas genom **IFG GEO Optimizer** är:

**IFG eCommerce** — baserad i Rom, Italien
E-post: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Vad vi samlar in

- **Handlarens kontodata (via Shopify OAuth)**: din butiksdomän, en API-åtkomsttoken och e-postadressen på ditt Shopify-konto.
- **Katalogdata (skrivskyddad)**: produkttitlar, beskrivningar, leverantör, priser, alternativ och tekniska specifikationer — används för att köra audits, simulera crawler-beteende, poängsätta innehållsextraherbarhet och utforma FAQ eller omskrivna beskrivningar.
- **Butikskonfiguration**: din aktiva plan, retur- och fraktpolicyuppgifterna och företagsdata du anger i Settings, sparade audits, FAQ- och innehållsomskrivningsutkast, samt de prompter du väljer att spåra för AI-synlighet.
- **Supportchattmeddelanden**: texten du utbyter med AI-assistenten i appen, inklusive transkriptet som vidarebefordras till oss om du uttryckligen ber om att få prata med en människa.
- **Anonym butiksfrontstrafik (Web Pixel, Grow/Unlimited)**: när en besökare kommer till en produktsida från en känd AI-motor (ChatGPT, Perplexity, Claude, Gemini, Copilot) registrerar vi motorn, sid-URL:en och en tidsstämpel — bara om besökaren redan gett analyssamtycke via din butiks cookiebanner. Ingen besökaridentifierare, cookie eller sessionsdata samlas in.
- **Teknisk data**: begärandetidsstämplar, interna postidentifierare och systemloggar.

> Appen **begär eller tar aldrig emot personlig slutkunddata** — inga namn, e-postadresser, adresser eller ordrar. De Shopify-behörigheter som begärs är `read_products`, `write_products` (katalog och strukturerad data), `read_themes` (kontroll av att temainbäddningen är aktiv) och `write_pixels` (aktivering av den anonyma trafikpixeln ovan).

## 3. Varför vi behandlar den, och på vilken rättslig grund

Vi behandlar denna data för att tillhandahålla tjänsten du installerade appen för — enligt Art. 6(1)(b) GDPR, fullgörande av avtal: analysera och förbättra din katalogs synlighet på generativa sökmotorer, inklusive AI-assisterad FAQ-utformning och omskrivning av innehåll, supportchatten i appen, veckovis AI-synlighetsspårning på prompter du väljer, och anonym mätning av AI-hänvisningstrafik — alla antingen initierade av handlaren eller, för trafikpixeln, samtyckesstyrda i din butiksfront.

## 4. Hur vi samlar in den

Kontodata samlas in en gång, genom Shopifys OAuth-flöde, vid installation. Katalogdata läses genom Shopifys Admin API endast när du utlöser en åtgärd från dashboarden. Trafikpixeln körs i din butiksfront och rapporterar händelser endast efter samtycke; inget annat körs i bakgrunden utan att du ber om det.

## 5. Vem vi delar den med

- **Google Firebase / Cloud Firestore** — lagrar din konfiguration, sessioner och utkast. Google LLC (USA) deltar i EU-US Data Privacy Framework. Data lagras i regionen europe-west1 (Belgien).
- **Anthropic PBC (USA)** — tillhandahåller Claude-modellen som används för FAQ-utformning, omskrivning av innehåll och supportchatten i appen, endast vid din uttryckliga åtgärd. Tar emot endast de produktattribut eller chattext du tillhandahåller — aldrig kunddata.
- **OpenAI, Inc. (USA)** och **Perplexity AI, Inc. (USA)** — används uteslutande för veckovis AI-synlighetsspårning på de prompter du uttryckligen väljer att övervaka. Tar emot endast den spårade prompttexten — aldrig kunddata.
- **Google LLC (USA)** — tillhandahåller Gemini-modellen, används på samma sätt som OpenAI/Perplexity ovan för synlighetsspårning (en separat användning från Firebase/Firestore, som endast är lagring).
- **Resend, Inc. (USA)** — skickar oss en notifiering, med butiksnamnet och supportchattens transkript, endast när du uttryckligen ber om att få prata med en människa i supportchatten.
- **Shopify Inc.** — plattformen själv, och källan till Admin API och Web Pixel-infrastrukturen som appen använder.

Vi säljer inte data, och vi använder den inte för marknadsföring eller beteendeprofilering.

## 6. Hur länge vi behåller den

- **Sessionstoken**: hanteras av Shopifys livscykel för offline-token, roteras automatiskt.
- **Konfiguration, audits, utkast och trafikhändelser**: behålls så länge appen är installerad. Avinstallation utlöser Shopifys `shop/redact`-webhook, som raderar din butiks konfiguration och sessioner helt.
- **Tekniska loggar**: behålls enligt Google Clouds standardlagringspolicy för loggar.

## 7. Dina rättigheter

Enligt Artikel 15–22 GDPR kan du begära tillgång till din data, rättelse av felaktig data, eller radering — det enklaste sättet är att avinstallera appen — eller invända mot behandlingen. Du kan även lämna in ett klagomål till din lokala tillsynsmyndighet för dataskydd. Eftersom appen aldrig behandlar personlig slutkunddata svarar efterlevnadswebhookarna `customers/data_request` och `customers/redact` med bekräftelse på att det inte finns något att exportera eller radera.

## 8. Säkerhet

All trafik går över HTTPS/TLS 1.2+. Shopifys autentiseringstoken exponeras aldrig för webbläsaren. Varje webhook verifieras med en konstanttids-HMAC SHA-256-kontroll innan den behandlas. Databasen är endast nåbar från backend, autentiserad via värdplattformens egen tjänsteidentitet — det finns inga statiska autentiseringsuppgifter i koden, och direkt klientåtkomst nekas av databasens egna säkerhetsregler. Data krypteras både i vila och under överföring.

## 9. Ändringar

Vi kan uppdatera denna policy från tid till annan. Väsentliga ändringar återspeglas här, med datumet högst upp hållet aktuellt.

---

**Frågor om din data?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Tillbaka till Hjälpcenter](index.html)
