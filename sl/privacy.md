---
title: IFG GEO Optimizer
description: Dokumentacija, pogosta vprašanja in pravne strani za Shopify aplikacijo IFG GEO Optimizer.
lang: sl
---

# Politika zasebnosti

<div class="lang-switcher">
{% include lang-switcher.html current="sl" slug="privacy" %}
</div>

**IFG GEO Optimizer** — aplikacija Shopify za Generative Engine Optimization
Nazadnje posodobljeno: julij 2026

## 1. Upravljavec podatkov

Upravljavec osebnih podatkov, obdelanih prek aplikacije **IFG GEO Optimizer**, je:

**IFG eCommerce** — s sedežem v Rimu, Italija
E-pošta: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Kaj zbiramo

- **Podatki o računu trgovca (prek Shopify OAuth)**: domena vaše trgovine, žeton za dostop do API in e-poštni naslov vašega računa Shopify.
- **Podatki kataloga (samo za branje)**: naslovi izdelkov, opisi, dobavitelj, cene, možnosti in tehnične specifikacije — uporabljeni za izvajanje revizij, simulacijo obnašanja pajkov, oceno izluščljivosti vsebine ter pripravo osnutkov pogostih vprašanj ali preoblikovanih opisov.
- **Konfiguracija trgovine**: vaš aktivni paket, podrobnosti politike vračil in dostave ter podatki o podjetju, ki jih vnesete v Nastavitvah, shranjene revizije, osnutki pogostih vprašanj in preoblikovane vsebine ter pozivi, ki jih izberete za sledenje vidnosti AI.
- **Sporočila klepeta podpore**: besedilo, ki ga izmenjate z asistentom AI v aplikaciji, vključno s prepisom, posredovanim nam, če izrecno zaprosite za pogovor s človekom.
- **Anonimni promet spletne trgovine (Web Pixel, Grow/Unlimited)**: ko obiskovalec pride na stran izdelka iz prepoznanega sistema AI (ChatGPT, Perplexity, Claude, Gemini, Copilot), zabeležimo sistem, URL strani in časovni žig — samo če je obiskovalec že podal privolitev za analitiko prek pasice s piškotki vaše trgovine. Noben identifikator obiskovalca, piškotek ali podatek o seji se ne zbira.
- **Tehnični podatki**: časovni žigi zahtev, notranji identifikatorji zapisov in sistemski dnevniki.

> Aplikacija **nikoli ne zahteva niti ne prejema osebnih podatkov končnih strank** — brez imen, e-poštnih naslovov, naslovov ali naročil. Zahtevana dovoljenja Shopify so `read_products`, `write_products` (katalog in strukturirani podatki), `read_themes` (preverjanje, ali je vgrajeni element teme aktiven) in `write_pixels` (aktivacija zgoraj omenjenega anonimnega piksela prometa).

## 3. Zakaj to obdelujemo in na kakšni pravni podlagi

Te podatke obdelujemo za zagotavljanje storitve, za katero ste namestili aplikacijo — na podlagi člena 6(1)(b) GDPR, izvajanje pogodbe: analiziranje in izboljševanje vidljivosti vašega kataloga na generativnih iskalnih sistemih, vključno s pomočjo AI pri pripravi pogostih vprašanj in preoblikovanju vsebine, klepetom podpore v aplikaciji, tedenskim sledenjem vidnosti AI pri pozivih, ki jih izberete, ter anonimnim merjenjem napotitvenega prometa iz AI — vse bodisi na pobudo trgovca, bodisi (pri pikslu prometa) pogojeno s privolitvijo v vaši spletni trgovini.

## 4. Kako to zbiramo

Podatki o računu se zberejo enkrat, prek postopka Shopify OAuth, ob namestitvi. Podatki kataloga se berejo prek Admin API Shopify samo, ko sprožite dejanje z nadzorne plošče. Piksel prometa deluje v vaši spletni trgovini in poroča dogodke samo po privolitvi; nič drugega ne deluje v ozadju, ne da bi za to zaprosili.

## 5. S kom to delimo

- **Google Firebase / Cloud Firestore** — shranjuje vašo konfiguracijo, seje in osnutke. Google LLC (ZDA) sodeluje v okviru EU-US Data Privacy Framework. Podatki so shranjeni v regiji europe-west1 (Belgija).
- **Anthropic PBC (ZDA)** — zagotavlja model Claude, uporabljen za pripravo pogostih vprašanj, preoblikovanje vsebine in klepet podpore v aplikaciji, izključno na vaše izrecno dejanje. Prejme le atribute izdelka ali besedilo klepeta, ki ga posredujete — nikoli podatkov o strankah.
- **OpenAI, Inc. (ZDA)** in **Perplexity AI, Inc. (ZDA)** — uporabljena izključno za tedensko sledenje vidnosti AI pri pozivih, ki jih izrecno izberete za spremljanje. Prejmeta le besedilo spremljanega poziva — nikoli podatkov o strankah.
- **Google LLC (ZDA)** — zagotavlja model Gemini, uporabljen na enak način kot OpenAI/Perplexity zgoraj za sledenje vidnosti (ločena uporaba od Firebase/Firestore, ki služi samo shranjevanju).
- **Resend, Inc. (ZDA)** — nam pošlje obvestilo, z imenom trgovine in prepisom klepeta podpore, izključno kadar izrecno zaprosite za pogovor s človekom v klepetu podpore.
- **Shopify Inc.** — sama platforma in vir infrastrukture Admin API ter Web Pixel, ki ju aplikacija uporablja.

Podatkov ne prodajamo in jih ne uporabljamo za trženje ali vedenjsko profiliranje.

## 6. Kako dolgo jih hranimo

- **Žetoni seje**: upravljani po življenjskem ciklu offline žetonov Shopify, samodejno se obnavljajo.
- **Konfiguracija, revizije, osnutki in dogodki prometa**: hranjeni, dokler je aplikacija nameščena. Odstranitev sproži webhook `shop/redact` Shopify, ki v celoti izbriše konfiguracijo in seje vaše trgovine.
- **Tehnični dnevniki**: hranjeni v skladu s standardno politiko hrambe dnevnikov Google Cloud.

## 7. Vaše pravice

V skladu s členi 15–22 GDPR lahko zahtevate dostop do svojih podatkov, popravek netočnih podatkov ali izbris — najpreprostejši način je odstranitev aplikacije — ali ugovarjate obdelavi. Pritožbo lahko vložite tudi pri lokalnem organu za varstvo podatkov. Ker aplikacija nikoli ne obdeluje osebnih podatkov končnih strank, webhooka za skladnost `customers/data_request` in `customers/redact` odgovorita s potrditvijo, da ni ničesar za izvoz ali izbris.

## 8. Varnost

Ves promet poteka prek HTTPS/TLS 1.2+. Avtentikacijski žetoni Shopify nikoli niso izpostavljeni brskalniku. Vsak webhook je pred obdelavo preverjen s konstantno-časovnim preverjanjem HMAC SHA-256. Baza podatkov je dosegljiva samo iz zalednega sistema, avtenticirana prek lastne identitete storitve gostiteljske platforme — v kodi ni statičnih poverilnic, neposreden dostop odjemalcev pa je onemogočen z lastnimi varnostnimi pravili baze podatkov. Podatki so šifrirani med mirovanjem in prenosom.

## 9. Spremembe

To politiko lahko občasno posodobimo. Bistvene spremembe bodo odražene tukaj, z datumom na vrhu, ki bo vedno posodobljen.

---

**Vprašanja o vaših podatkih?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Nazaj v Center za pomoč](index.html)
