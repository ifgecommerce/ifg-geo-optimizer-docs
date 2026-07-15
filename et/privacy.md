---
title: IFG GEO Optimizer
description: Shopify rakenduse IFG GEO Optimizer dokumentatsioon, KKK ja õiguslikud leheküljed.
lang: et
---

# Privaatsuspoliitika

<div class="lang-switcher">
{% include lang-switcher.html current="et" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify rakendus generatiivsete mootorite optimeerimiseks (Generative Engine Optimization)
Viimati uuendatud: juuli 2026

## 1. Vastutav töötleja

Isikuandmete vastutav töötleja, mida töödeldakse **IFG GEO Optimizeri** kaudu, on:

**IFG eCommerce** — asukohaga Roomas, Itaalias
E-post: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Mida me kogume

- **Kaupleja konto andmed (Shopify OAuth kaudu)**: sinu poe domeen, API juurdepääsutoken ja sinu Shopify konto e-posti aadress.
- **Kataloogi andmed (ainult lugemiseks)**: toote pealkirjad, kirjeldused, tootja, hinnad, valikud ja tehnilised andmed — kasutatakse auditite läbiviimiseks, crawleri käitumise simuleerimiseks, sisu eraldatavuse hindamiseks ning KKK-de või ümberkirjutatud kirjelduste koostamiseks.
- **Poe seadistus**: sinu aktiivne pakett, tagastus- ja tarnepoliitika andmed ning ettevõtte andmed, mille sisestad Settings alla, salvestatud auditid, KKK ja sisu ümberkirjutamise mustandid, ning päringud, mida valid AI nähtavuse jälgimiseks.
- **Tugivestluse sõnumid**: tekst, mida vahetad rakendusesisese AI assistendiga, sealhulgas vestluse ülekanne, mis edastatakse meile, kui selgesõnaliselt palud inimesega rääkida.
- **Anonüümne poe liiklus (Web Pixel, Grow/Unlimited)**: kui külastaja saabub tootelehele tuntud AI mootorist (ChatGPT, Perplexity, Claude, Gemini, Copilot), salvestame mootori, lehe URL-i ja ajatempli — ainult siis, kui külastaja on juba andnud analüütika nõusoleku sinu poe küpsisebänneri kaudu. Ühtegi külastaja identifikaatorit, küpsist ega seansiandmeid ei koguta.
- **Tehnilised andmed**: päringute ajatemplid, sisemised kirje identifikaatorid ja süsteemi logid.

> Rakendus **ei küsi ega saa kunagi lõppkliendi isikuandmeid** — ei nimesid, e-poste, aadresse ega tellimusi. Küsitavad Shopify õigused on `read_products`, `write_products` (kataloog ja struktureeritud andmed), `read_themes` (teema manuse aktiivsuse kontrollimine) ja `write_pixels` (ülalnimetatud anonüümse liiklusepiksli aktiveerimine).

## 3. Miks me seda töötleme ja millisel õiguslikul alusel

Töötleme neid andmeid, et osutada teenust, mille jaoks rakenduse paigaldasid — vastavalt Isikuandmete kaitse üldmääruse (GDPR) art. 6(1)(b), lepingu täitmine: sinu kataloogi nähtavuse analüüsimine ja parandamine generatiivsetes otsingumootorites, sealhulgas AI-abistatud KKK koostamine ja sisu ümberkirjutamine, rakendusesisene tugivestlus, iganädalane AI-nähtavuse jälgimine sinu valitud päringutel, ning anonüümne AI-suunatud liikluse mõõtmine — kõik kas kaupleja algatatud või, liiklusepiksli puhul, nõusolekust sõltuv sinu e-poes.

## 4. Kuidas me seda kogume

Konto andmed kogutakse üks kord, Shopify OAuth voo kaudu, paigaldamisel. Kataloogi andmeid loetakse Shopify Admin API kaudu ainult siis, kui käivitad toimingu töölaualt. Liiklusepiksel töötab sinu e-poes ja raporteerib sündmusi ainult pärast nõusolekut; miski muu ei tööta taustal ilma sinu poolse päringuta.

## 5. Kellega me seda jagame

- **Google Firebase / Cloud Firestore** — salvestab sinu seadistuse, seansid ja mustandid. Google LLC (USA) osaleb ELi-USA andmekaitseraamistikus (EU-US Data Privacy Framework). Andmed säilitatakse europe-west1 piirkonnas (Belgia).
- **Anthropic PBC (USA)** — pakub Claude mudelit, mida kasutatakse KKK koostamiseks, sisu ümberkirjutamiseks ja rakendusesiseseks tugivestluseks, ainult sinu selgesõnalisel tegevusel. Saab ainult tooteatribuudid või vestlusteksti, mida sina esitad — mitte kunagi kliendiandmeid.
- **OpenAI, Inc. (USA)** ja **Perplexity AI, Inc. (USA)** — kasutatakse ainult iganädalaseks AI-nähtavuse jälgimiseks päringutel, mida sina selgesõnaliselt valid jälgimiseks. Saavad ainult jälgitava päringu teksti — mitte kunagi kliendiandmeid.
- **Google LLC (USA)** — pakub Gemini mudelit, mida kasutatakse samamoodi nagu OpenAI/Perplexity ülalpool nähtavuse jälgimiseks (eraldiseisev kasutus võrreldes Firebase/Firestore'iga, mis on ainult salvestamiseks).
- **Resend, Inc. (USA)** — saadab meile teavituse koos poe nime ja tugivestluse ülekandega, ainult siis, kui selgesõnaliselt palud tugivestluses inimesega rääkida.
- **Shopify Inc.** — platvorm ise ning Admin API ja Web Pixel infrastruktuuri allikas, mida rakendus kasutab.

Me ei müü andmeid ega kasuta neid turunduseks ega käitumusliku profileerimise jaoks.

## 6. Kui kaua me seda säilitame

- **Seansi tokenid**: hallatakse Shopify offline-tokeni elutsükli kaudu, uuendatakse automaatselt.
- **Seadistus, auditid, mustandid ja liiklussündmused**: säilitatakse seni, kuni rakendus on paigaldatud. Desinstallimine käivitab Shopify `shop/redact` veebihaagi (webhook), mis kustutab sinu poe seadistuse ja seansid täielikult.
- **Tehnilised logid**: säilitatakse vastavalt Google Cloudi standardsele logi säilitamise poliitikale.

## 7. Sinu õigused

Vastavalt GDPR artiklitele 15–22 saad taotleda ligipääsu oma andmetele, ebatäpsete andmete parandamist või kustutamist — lihtsaim viis on rakendus desinstallida — või vastuväiteid töötlemisele. Samuti saad esitada kaebuse oma kohalikule andmekaitseasutusele. Kuna rakendus ei töötle kunagi lõppkliendi isikuandmeid, vastavad vastavusveebihaagid `customers/data_request` ja `customers/redact` kinnitusega, et pole midagi eksportida ega kustutada.

## 8. Turvalisus

Kogu liiklus toimub HTTPS/TLS 1.2+ kaudu. Shopify autentimistokeneid ei avaldata kunagi brauserile. Iga veebihaak kontrollitakse konstantse ajaga HMAC SHA-256 kontrolliga enne töötlemist. Andmebaas on ligipääsetav ainult taustasüsteemist, autenditud majutusplatvormi enda teenuse identiteedi kaudu — koodis pole staatilisi mandaate ning otsene kliendipoolne ligipääs on andmebaasi enda turvareeglitega keelatud. Andmed on krüpteeritud nii puhkeolekus kui ka edastamisel.

## 9. Muudatused

Võime seda poliitikat aeg-ajalt uuendada. Olulised muudatused kajastuvad siin, ülal oleva kuupäevaga ajakohasena hoituna.

---

**Küsimused oma andmete kohta?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Tagasi Abikeskusesse](index.html)
