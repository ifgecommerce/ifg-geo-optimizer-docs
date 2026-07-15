---
title: IFG GEO Optimizer
description: Dokumentacija, česta pitanja i pravne stranice za Shopify aplikaciju IFG GEO Optimizer.
lang: hr
---

# Pravila privatnosti

<div class="lang-switcher">
{% include lang-switcher.html current="hr" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify aplikacija za Generative Engine Optimization
Zadnje ažurirano: srpanj 2026.

## 1. Voditelj obrade podataka

Voditelj obrade osobnih podataka koji se obrađuju putem aplikacije **IFG GEO Optimizer** je:

**IFG eCommerce** — sa sjedištem u Rimu, Italija
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Što prikupljamo

- **Podaci o računu trgovca (putem Shopify OAuth)**: domena vaše trgovine, API pristupni token i e-mail adresa vezana uz vaš Shopify račun.
- **Podaci kataloga (samo za čitanje)**: nazivi proizvoda, opisi, dobavljač, cijene, opcije i tehničke specifikacije — koriste se za pokretanje audita, simuliranje ponašanja crawlera, ocjenjivanje ekstraktibilnosti sadržaja i sastavljanje FAQ-a ili prepisanih opisa.
- **Konfiguracija trgovine**: vaš aktivni plan, detalji politike povrata i dostave te podaci o tvrtki koje unosite u Postavkama, spremljeni auditi, nacrti FAQ-a i prepisanog sadržaja, te upiti koje odaberete za praćenje AI vidljivosti.
- **Poruke chat podrške**: tekst koji razmjenjujete s AI asistentom unutar aplikacije, uključujući transkript koji nam se prosljeđuje ako izričito zatražite razgovor s čovjekom.
- **Anonimni promet trgovine (Web Pixel, Grow/Unlimited)**: kada posjetitelj dođe na stranicu proizvoda s prepoznatog AI motora (ChatGPT, Perplexity, Claude, Gemini, Copilot), bilježimo motor, URL stranice i vremensku oznaku — samo ako je posjetitelj već dao pristanak za analitiku putem bannera kolačića vaše trgovine. Ne prikuplja se nikakav identifikator posjetitelja, kolačić ni podatak o sesiji.
- **Tehnički podaci**: vremenske oznake zahtjeva, interni identifikatori zapisa i sistemski zapisnici (logovi).

> Aplikacija **nikada ne zahtijeva niti prima osobne podatke krajnjih kupaca** — nikakva imena, e-mailove, adrese ili narudžbe. Zatražene Shopify dozvole su `read_products`, `write_products` (katalog i strukturirani podaci), `read_themes` (provjera je li embed teme aktivan) i `write_pixels` (aktivacija gore navedenog anonimnog piksela prometa).

## 3. Zašto ih obrađujemo i po kojoj pravnoj osnovi

Ove podatke obrađujemo kako bismo pružili uslugu radi koje ste instalirali aplikaciju — na temelju čl. 6(1)(b) GDPR-a, izvršenje ugovora: analiza i poboljšanje vidljivosti vašeg kataloga na generativnim tražilicama, uključujući AI-asistirano sastavljanje FAQ-a i prepisivanje sadržaja, chat podršku unutar aplikacije, tjedno praćenje AI vidljivosti na upitima koje odaberete, te mjerenje anonimnog AI referral prometa — sve inicirano od strane trgovca ili, za piksel prometa, uvjetovano pristankom na vašoj trgovini.

## 4. Kako ih prikupljamo

Podaci o računu prikupljaju se jednom, putem Shopify OAuth procesa, prilikom instalacije. Podaci kataloga čitaju se putem Shopify Admin API-ja samo kada pokrenete radnju s dashboarda. Piksel prometa radi na vašoj trgovini i izvještava o događajima samo nakon pristanka; ništa se drugo ne izvršava u pozadini bez vašeg izričitog zahtjeva.

## 5. S kim ih dijelimo

- **Google Firebase / Cloud Firestore** — pohranjuje vašu konfiguraciju, sesije i nacrte. Google LLC (SAD) sudjeluje u EU-US Data Privacy Frameworku. Podaci se pohranjuju u regiji europe-west1 (Belgija).
- **Anthropic PBC (SAD)** — pruža Claude model korišten za sastavljanje FAQ-a, prepisivanje sadržaja i chat podršku unutar aplikacije, samo na vašu izričitu akciju. Prima samo atribute proizvoda ili tekst chata koje vi dostavite — nikada podatke o kupcima.
- **OpenAI, Inc. (SAD)** i **Perplexity AI, Inc. (SAD)** — koriste se isključivo za tjedno praćenje AI vidljivosti na upitima koje izričito odaberete za nadzor. Primaju samo tekst praćenog upita — nikada podatke o kupcima.
- **Google LLC (SAD)** — pruža Gemini model, korišten na isti način kao OpenAI/Perplexity gore, za praćenje vidljivosti (odvojena upotreba od Firebase/Firestore, koji služi samo za pohranu).
- **Resend, Inc. (SAD)** — šalje nam obavijest, s nazivom trgovine i transkriptom chat podrške, samo kada izričito zatražite razgovor s čovjekom u chatu podrške.
- **Shopify Inc.** — sama platforma i izvor Admin API-ja i infrastrukture Web Pixela koju aplikacija koristi.

Ne prodajemo podatke i ne koristimo ih za marketing ni bihevioralno profiliranje.

## 6. Koliko dugo ih čuvamo

- **Sesijski tokeni**: upravljani Shopify životnim ciklusom offline tokena, automatski se rotiraju.
- **Konfiguracija, auditi, nacrti i događaji prometa**: čuvaju se dok god je aplikacija instalirana. Deinstalacija pokreće Shopify webhook `shop/redact`, koji u potpunosti briše konfiguraciju i sesije vaše trgovine.
- **Tehnički zapisnici**: čuvaju se sukladno standardnom razdoblju čuvanja zapisnika Google Clouda.

## 7. Vaša prava

Sukladno člancima 15–22 GDPR-a, možete zatražiti pristup svojim podacima, ispravak netočnih podataka ili brisanje — najjednostavniji način je deinstalacija aplikacije — ili prigovor na obradu. Također možete podnijeti pritužbu svom lokalnom tijelu za zaštitu podataka. Budući da aplikacija nikada ne obrađuje osobne podatke krajnjih kupaca, compliance webhookovi `customers/data_request` i `customers/redact` odgovaraju potvrdom da nema ničega za izvoz ili brisanje.

## 8. Sigurnost

Sav promet odvija se putem HTTPS/TLS 1.2+. Shopify autentikacijski tokeni nikada nisu izloženi pregledniku. Svaki webhook provjerava se HMAC SHA-256 provjerom u konstantnom vremenu prije obrade. Baza podataka dostupna je samo backendu, autenticirana putem vlastitog servisnog identiteta hosting platforme — u kodu nema statičkih vjerodajnica, a izravan pristup klijenta odbijen je vlastitim sigurnosnim pravilima baze podataka. Podaci su enkriptirani u mirovanju i tijekom prijenosa.

## 9. Izmjene

Ova pravila možemo s vremena na vrijeme ažurirati. Značajne izmjene bit će prikazane ovdje, s datumom na vrhu koji se održava ažurnim.

---

**Pitanja o vašim podacima?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Natrag na Centar za pomoć](index.html)
