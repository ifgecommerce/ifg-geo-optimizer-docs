---
title: IFG GEO Optimizer
description: „IFG GEO Optimizer“ Shopify programos dokumentacija, DUK ir teisiniai puslapiai.
lang: lt
---

# Privatumo politika

<div class="lang-switcher">
{% include lang-switcher.html current="lt" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify programa, skirta Generative Engine Optimization
Paskutinį kartą atnaujinta: 2026 m. liepa

## 1. Duomenų valdytojas

Asmens duomenų, tvarkomų per **IFG GEO Optimizer**, valdytojas yra:

**IFG eCommerce** — įsikūrusi Romoje, Italijoje
El. paštas: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Ką renkame

- **Prekybininko paskyros duomenys (per Shopify OAuth)**: jūsų parduotuvės domenas, API prieigos raktas ir el. pašto adresas, susietas su jūsų Shopify paskyra.
- **Katalogo duomenys (tik skaitymui)**: produktų pavadinimai, aprašymai, tiekėjas, kainos, parinktys ir techninės specifikacijos — naudojami auditams atlikti, crawler'io elgsenai simuliuoti, turinio išgaunamumui vertinti ir DUK ar perrašytiems aprašymams rengti.
- **Parduotuvės konfigūracija**: jūsų aktyvus planas, grąžinimo ir siuntimo politikos duomenys bei įmonės informacija, kuriuos įvedate Settings skiltyje, išsaugoti auditai, DUK ir turinio perrašymo juodraščiai, ir užklausos, kurias pasirenkate stebėti AI matomumui.
- **Pagalbos pokalbio žinutės**: tekstas, kuriuo apsikeičiate su programos viduje veikiančiu AI asistentu, įskaitant pokalbio įrašą, persiunčiamą mums, jei aiškiai paprašote pakalbėti su žmogumi.
- **Anoniminis parduotuvės vitrinos srautas (Web Pixel, Grow/Unlimited)**: kai lankytojas į produkto puslapį atkeliauja iš atpažinto AI variklio (ChatGPT, Perplexity, Claude, Gemini, Copilot), užfiksuojame variklį, puslapio URL ir laiko žymą — tik jei lankytojas jau davė sutikimą analitikai per jūsų parduotuvės slapukų juostą. Joks lankytojo identifikatorius, slapukas ar sesijos duomenys nerenkami.
- **Techniniai duomenys**: užklausų laiko žymos, vidiniai įrašų identifikatoriai ir sistemos žurnalai.

> Programa **niekada neprašo ir negauna asmeninių galutinio kliento duomenų** — jokių vardų, el. pašto adresų, adresų ar užsakymų. Prašomi Shopify leidimai yra `read_products`, `write_products` (katalogas ir struktūrizuoti duomenys), `read_themes` (temos priedo aktyvavimo patikra) ir `write_pixels` (aukščiau minėto anoniminio srauto pikselio aktyvavimas).

## 3. Kodėl tai tvarkome ir kokiu teisiniu pagrindu

Šiuos duomenis tvarkome tam, kad suteiktume paslaugą, dėl kurios įsidiegėte programą — pagal GDPR 6 str. 1 d. b) punktą, sutarties vykdymą: jūsų katalogo matomumo generatyviuose paieškos varikliuose analizę ir gerinimą, įskaitant AI padedamą DUK rengimą ir turinio perrašymą, pagalbos pokalbį programoje, savaitinį AI matomumo stebėjimą pagal jūsų pasirinktas užklausas, ir anoniminį AI nukreipiamo srauto matavimą — visa tai inicijuoja prekybininkas arba, srauto pikselio atveju, priklauso nuo sutikimo jūsų parduotuvės vitrinoje.

## 4. Kaip tai renkame

Paskyros duomenys renkami vieną kartą, per Shopify OAuth procesą, diegimo metu. Katalogo duomenys nuskaitomi per Shopify Admin API tik tada, kai inicijuojate veiksmą iš dashboard. Srauto pikselis veikia jūsų parduotuvės vitrinoje ir praneša įvykius tik po sutikimo; niekas kitas fone neveikia be jūsų prašymo.

## 5. Su kuo jais dalijamės

- **Google Firebase / Cloud Firestore** — saugo jūsų konfigūraciją, sesijas ir juodraščius. „Google LLC“ (JAV) dalyvauja ES–JAV duomenų privatumo sistemoje (EU-US Data Privacy Framework). Duomenys saugomi europe-west1 regione (Belgija).
- **Anthropic PBC (JAV)** — teikia Claude modelį, naudojamą DUK rengimui, turinio perrašymui ir pagalbos pokalbiui programoje, tik jums aiškiai atlikus veiksmą. Gauna tik jūsų pateiktus produkto atributus ar pokalbio tekstą — niekada kliento duomenų.
- **OpenAI, Inc. (JAV)** ir **Perplexity AI, Inc. (JAV)** — naudojami išimtinai savaitiniam AI matomumo stebėjimui pagal užklausas, kurias aiškiai pasirenkate stebėti. Gauna tik stebimos užklausos tekstą — niekada kliento duomenų.
- **Google LLC (JAV)** — teikia Gemini modelį, naudojamą tuo pačiu būdu kaip OpenAI/Perplexity aukščiau, matomumo stebėjimui (atskira paskirtis nuo Firebase/Firestore, kuri naudojama tik saugojimui).
- **Resend, Inc. (JAV)** — siunčia mums pranešimą su parduotuvės pavadinimu ir pagalbos pokalbio įrašu, tik kai aiškiai paprašote pagalbos pokalbyje pakalbėti su žmogumi.
- **Shopify Inc.** — pati platforma ir Admin API bei Web Pixel infrastruktūros, kurias naudoja programa, šaltinis.

Duomenų neparduodame ir nenaudojame rinkodarai ar elgsenos profiliavimui.

## 6. Kiek laiko juos saugome

- **Sesijos žetonai (tokens)**: valdomi pagal Shopify offline žetono gyvavimo ciklą, rotuojami automatiškai.
- **Konfigūracija, auditai, juodraščiai ir srauto įvykiai**: saugomi tol, kol programa įdiegta. Pašalinimas suaktyvina Shopify `shop/redact` webhook'ą, kuris visiškai ištrina jūsų parduotuvės konfigūraciją ir sesijas.
- **Techniniai žurnalai**: saugomi pagal standartinį Google Cloud žurnalų saugojimo laikotarpį.

## 7. Jūsų teisės

Pagal GDPR 15–22 straipsnius galite paprašyti prieigos prie savo duomenų, netikslių duomenų taisymo ar ištrynimo — paprasčiausias būdas yra pašalinti programą — arba paprieštarauti duomenų tvarkymui. Taip pat galite pateikti skundą savo vietinei duomenų apsaugos institucijai. Kadangi programa niekada netvarko asmeninių galutinio kliento duomenų, `customers/data_request` ir `customers/redact` atitikties webhook'ai atsako patvirtindami, kad eksportuoti ar ištrinti nėra ko.

## 8. Saugumas

Visas srautas veikia per HTTPS/TLS 1.2+. Shopify autentifikacijos žetonai niekada neatskleidžiami naršyklei. Kiekvienas webhook prieš apdorojimą tikrinamas pastoviu laiku (constant-time) HMAC SHA-256 patikra. Duomenų bazė pasiekiama tik iš backend, autentifikuota per pačios prieglobos platformos paslaugos tapatybę — kode nėra jokių statinių prisijungimo duomenų, o tiesioginė kliento prieiga draudžiama pačios duomenų bazės saugumo taisyklėmis. Duomenys šifruojami tiek saugojimo, tiek perdavimo metu.

## 9. Pakeitimai

Šią politiką galime laikas nuo laiko atnaujinti. Esminiai pakeitimai bus atspindėti čia, o data viršuje bus nuolat atnaujinama.

---

**Klausimai apie savo duomenis?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Atgal į Pagalbos centrą](index.html)
