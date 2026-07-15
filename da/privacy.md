---
title: IFG GEO Optimizer
description: Dokumentation, FAQ og juridiske sider til Shopify-appen IFG GEO Optimizer.
lang: da
---

# Privatlivspolitik

<div class="lang-switcher">
{% include lang-switcher.html current="da" slug="privacy" %}
</div>

**IFG GEO Optimizer** — en Shopify-app til Generative Engine Optimization
Senest opdateret: juli 2026

## 1. Dataansvarlig

Den dataansvarlige for personoplysninger, der behandles gennem **IFG GEO Optimizer**, er:

**IFG eCommerce** — hjemmehørende i Rom, Italien
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Hvad vi indsamler

- **Forhandlerkontodata (via Shopify OAuth)**: din butiksdomæne, en API-adgangstoken og e-mailadressen på din Shopify-konto.
- **Katalogdata (skrivebeskyttet)**: produkttitler, beskrivelser, leverandør, priser, valgmuligheder og tekniske specifikationer — bruges til at køre audits, simulere crawler-adfærd, score indholdsudtrækkelighed og udarbejde FAQ'er eller omskrevne beskrivelser.
- **Butikskonfiguration**: din aktive plan, detaljerne om returnerings- og forsendelsespolitik samt virksomhedsdata, du indtaster i Settings, gemte audits, FAQ- og content-rewrite-udkast, samt de prompts, du vælger at spore for AI-synlighed.
- **Supportchat-beskeder**: den tekst, du udveksler med AI-assistenten i appen, inklusive den transskription, der videresendes til os, hvis du udtrykkeligt beder om at tale med et menneske.
- **Anonym storefront-trafik (Web Pixel, Grow/Unlimited)**: når en besøgende ankommer til en produktside fra en genkendt AI-motor (ChatGPT, Perplexity, Claude, Gemini, Copilot), registrerer vi motoren, side-URL'en og et tidsstempel — kun hvis den besøgende allerede har givet analysesamtykke gennem din butiks cookiebanner. Ingen besøgende-identifikator, cookie eller sessiondata indsamles.
- **Tekniske data**: anmodningstidsstempler, interne postidentifikatorer og systemlogfiler.

> Appen **anmoder aldrig om eller modtager personlige slutkundedata** — ingen navne, e-mails, adresser eller ordrer. De Shopify-tilladelser, der anmodes om, er `read_products`, `write_products` (katalog og strukturerede data), `read_themes` (kontrol af at temaembedden er aktiv) og `write_pixels` (aktivering af den anonyme trafikpixel ovenfor).

## 3. Hvorfor vi behandler det, og under hvilket retsgrundlag

Vi behandler disse data for at levere den tjeneste, du installerede appen for — under Art. 6, stk. 1, litra b) GDPR, opfyldelse af en kontrakt: analyse og forbedring af dit katalogs synlighed på generative søgemaskiner, herunder AI-assisteret FAQ-udarbejdelse og omskrivning af indhold, supportchatten i appen, ugentlig AI-synlighedssporing på prompts du selv vælger, og anonym måling af AI-henvisningstrafik — alt sammen enten initieret af forhandleren eller, for trafikpixlen, betinget af samtykke på din storefront.

## 4. Hvordan vi indsamler det

Kontodata indsamles én gang, gennem Shopifys OAuth-flow, ved installation. Katalogdata læses gennem Shopifys Admin API kun, når du udløser en handling fra dashboardet. Trafikpixlen kører på din storefront og rapporterer hændelser kun efter samtykke; intet andet kører i baggrunden, uden at du beder om det.

## 5. Hvem vi deler det med

- **Google Firebase / Cloud Firestore** — gemmer din konfiguration, sessioner og udkast. Google LLC (USA) deltager i EU-US Data Privacy Framework. Data opbevares i regionen europe-west1 (Belgien).
- **Anthropic PBC (USA)** — leverer Claude-modellen, der bruges til FAQ-udarbejdelse, omskrivning af indhold og supportchatten i appen, kun ved din udtrykkelige handling. Modtager kun de produktattributter eller chattekst, du angiver — aldrig kundedata.
- **OpenAI, Inc. (USA)** og **Perplexity AI, Inc. (USA)** — bruges udelukkende til ugentlig AI-synlighedssporing på de prompts, du udtrykkeligt vælger at overvåge. Modtager kun den sporede prompt-tekst — aldrig kundedata.
- **Google LLC (USA)** — leverer Gemini-modellen, brugt på samme måde som OpenAI/Perplexity ovenfor til synlighedssporing (en anden brug end Firebase/Firestore, som udelukkende er lagring).
- **Resend, Inc. (USA)** — sender os en notifikation med butiksnavnet og supportchat-transskriptionen, kun når du udtrykkeligt beder om at tale med et menneske i supportchatten.
- **Shopify Inc.** — selve platformen, og kilden til Admin API'et og Web Pixel-infrastrukturen, appen bruger.

Vi sælger ikke data, og vi bruger dem ikke til markedsføring eller adfærdsprofilering.

## 6. Hvor længe vi opbevarer det

- **Sessiontokens**: administreres af Shopifys offline-token-livscyklus, roteres automatisk.
- **Konfiguration, audits, udkast og trafikhændelser**: opbevares, så længe appen er installeret. Afinstallation udløser Shopifys `shop/redact`-webhook, som sletter din butiks konfiguration og sessioner fuldstændigt.
- **Tekniske logfiler**: opbevares under Google Clouds standard logopbevaringsperiode.

## 7. Dine rettigheder

I henhold til artikel 15-22 GDPR kan du anmode om indsigt i dine data, berigtigelse af unøjagtige data eller sletning — den enkleste måde er at afinstallere appen — eller gøre indsigelse mod behandling. Du kan også indgive en klage til din lokale databeskyttelsesmyndighed. Da appen aldrig behandler personlige slutkundedata, svarer overensstemmelses-webhooksene `customers/data_request` og `customers/redact` med bekræftelse af, at der ikke er noget at eksportere eller slette.

## 8. Sikkerhed

Al trafik kører over HTTPS/TLS 1.2+. Shopify-godkendelsestokens eksponeres aldrig for browseren. Hver webhook verificeres med en HMAC SHA-256-kontrol med konstant tid, før den behandles. Databasen kan kun tilgås fra backend, godkendt via hostingplatformens egen serviceidentitet — der er ingen statiske adgangsoplysninger i koden, og direkte klientadgang afvises af databasens egne sikkerhedsregler. Data krypteres både under opbevaring og under overførsel.

## 9. Ændringer

Vi kan opdatere denne politik fra tid til anden. Væsentlige ændringer vil blive afspejlet her, med datoen øverst holdt ajour.

---

**Spørgsmål om dine data?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Tilbage til Hjælpecenter](index.html)
