---
title: IFG GEO Optimizer
description: Dokumentācija, BUJ un juridiskās lapas Shopify lietotnei IFG GEO Optimizer.
lang: lv
---

# Privātuma politika

<div class="lang-switcher">
{% include lang-switcher.html current="lv" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify lietotne Generative Engine Optimization vajadzībām
Pēdējoreiz atjaunināts: 2026. gada jūlijā

## 1. Datu pārzinis

Personas datu pārzinis, kas apstrādāti ar **IFG GEO Optimizer** starpniecību, ir:

**IFG eCommerce** — atrodas Romā, Itālijā
E-pasts: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Ko mēs vācam

- **Tirgotāja konta dati (caur Shopify OAuth)**: tava veikala domēns, API piekļuves marķieris (token) un e-pasta adrese, kas norādīta tavā Shopify kontā.
- **Kataloga dati (tikai lasīšanai)**: produktu nosaukumi, apraksti, ražotājs, cenas, opcijas un tehniskās specifikācijas — izmanto, lai veiktu auditus, simulētu crawler uzvedību, novērtētu satura izvelkamību un sagatavotu FAQ vai pārrakstītus aprakstus.
- **Veikala konfigurācija**: tavs aktīvais plāns, atgriešanas un piegādes politikas detaļas un uzņēmuma dati, ko ievadi sadaļā Settings, saglabātie audits, FAQ un satura pārrakstīšanas melnraksti, un uzvednes, ko izvēlies izsekot AI redzamībai.
- **Atbalsta tērzēšanas ziņas**: teksts, ko apmaini ar lietotnes iekšējo AI asistentu, tostarp saruna, kas tiek pārsūtīta mums, ja tieši lūdz runāt ar cilvēku.
- **Anonīms veikala apmeklējumu satiksmes dati (Web Pixel, Grow/Unlimited)**: kad apmeklētājs nonāk produkta lapā no atpazīta AI dzinēja (ChatGPT, Perplexity, Claude, Gemini, Copilot), mēs reģistrējam dzinēju, lapas URL un laika zīmogu — tikai tad, ja apmeklētājs jau devis analītikas piekrišanu caur tava veikala sīkdatņu joslu. Netiek vākts neviens apmeklētāja identifikators, sīkdatne vai sesijas dati.
- **Tehniskie dati**: pieprasījumu laika zīmogi, iekšējie ierakstu identifikatori un sistēmas žurnāli.

> Lietotne **nekad nepieprasa un nesaņem gala klientu personas datus** — nekādus vārdus, e-pastus, adreses vai pasūtījumus. Pieprasītās Shopify atļaujas ir `read_products`, `write_products` (katalogs un strukturētie dati), `read_themes` (pārbauda, vai tēmas embed ir aktīvs) un `write_pixels` (aktivizē iepriekš minēto anonīmo satiksmes pikseli).

## 3. Kāpēc mēs to apstrādājam un uz kāda juridiskā pamata

Mēs apstrādājam šos datus, lai sniegtu pakalpojumu, kura dēļ tu instalēji lietotni — saskaņā ar VDAR 6. panta 1. punkta b) apakšpunktu (līguma izpilde): tava kataloga redzamības analīze un uzlabošana ģeneratīvajās meklētājprogrammās, tostarp AI atbalstīta FAQ sagatavošana un satura pārrakstīšana, lietotnes iekšējā atbalsta tērzēšana, iknedēļas AI redzamības izsekošana uzvednēm, ko izvēlies, un anonīma AI ieteiktās satiksmes mērīšana — visas šīs darbības ir vai nu tirgotāja ierosinātas, vai — satiksmes pikseļa gadījumā — atkarīgas no piekrišanas tavā veikalā.

## 4. Kā mēs to vācam

Konta dati tiek vākti vienu reizi, instalācijas laikā, caur Shopify OAuth plūsmu. Kataloga dati tiek nolasīti caur Shopify Admin API tikai tad, kad ierosini darbību no paneļa (dashboard). Satiksmes pikselis darbojas tavā veikalā un ziņo notikumus tikai pēc piekrišanas saņemšanas; nekas cits fonā nedarbojas bez tava pieprasījuma.

## 5. Ar ko mēs to koplietojam

- **Google Firebase / Cloud Firestore** — glabā tavu konfigurāciju, sesijas un melnrakstus. Google LLC (ASV) piedalās ES-ASV Datu privātuma satvarā (EU-US Data Privacy Framework). Dati tiek glabāti europe-west1 reģionā (Beļģija).
- **Anthropic PBC (ASV)** — nodrošina Claude modeli, ko izmanto FAQ sagatavošanai, satura pārrakstīšanai un lietotnes iekšējai atbalsta tērzēšanai, tikai pēc tavas tiešas darbības. Saņem tikai produkta atribūtus vai tērzēšanas tekstu, ko sniedz — nekad klientu datus.
- **OpenAI, Inc. (ASV)** un **Perplexity AI, Inc. (ASV)** — izmanto tikai iknedēļas AI redzamības izsekošanai uzvednēm, ko tieši izvēlies uzraudzīt. Saņem tikai izsekotās uzvednes tekstu — nekad klientu datus.
- **Google LLC (ASV)** — nodrošina Gemini modeli, izmantots tāpat kā OpenAI/Perplexity iepriekš minētajai redzamības izsekošanai (atšķirīgs izmantojums no Firebase/Firestore, kas ir tikai glabāšana).
- **Resend, Inc. (ASV)** — nosūta mums paziņojumu ar veikala nosaukumu un atbalsta tērzēšanas sarunu, tikai tad, kad tieši lūdz runāt ar cilvēku atbalsta tērzēšanā.
- **Shopify Inc.** — pati platforma un Admin API un Web Pixel infrastruktūras avots, ko lietotne izmanto.

Mēs nepārdodam datus un neizmantojam tos mārketingam vai uzvedības profilēšanai.

## 6. Cik ilgi mēs tos glabājam

- **Sesijas marķieri (tokens)**: pārvalda Shopify offline-token dzīves cikls, tiek automātiski rotēti.
- **Konfigurācija, audits, melnraksti un satiksmes notikumi**: tiek glabāti, kamēr lietotne ir instalēta. Atinstalēšana ierosina Shopify `shop/redact` webhook, kas pilnībā dzēš tava veikala konfigurāciju un sesijas.
- **Tehniskie žurnāli**: tiek glabāti saskaņā ar Google Cloud standarta žurnālu glabāšanas politiku.

## 7. Tavas tiesības

Saskaņā ar VDAR 15.–22. pantu vari pieprasīt piekļuvi saviem datiem, neprecīzu datu labošanu vai dzēšanu — vienkāršākais veids ir atinstalēt lietotni — vai iebilst pret apstrādi. Vari arī iesniegt sūdzību savai vietējai datu aizsardzības uzraudzības iestādei. Tā kā lietotne nekad neapstrādā gala klientu personas datus, atbilstības webhooks `customers/data_request` un `customers/redact` atbild, apstiprinot, ka nav nekā, ko eksportēt vai dzēst.

## 8. Drošība

Visa satiksme notiek caur HTTPS/TLS 1.2+. Shopify autentifikācijas marķieri (tokens) nekad netiek atklāti pārlūkam. Katrs webhook tiek pārbaudīts ar konstanta laika HMAC SHA-256 pārbaudi, pirms tas tiek apstrādāts. Datubāze ir pieejama tikai no backend, autentificēta ar mitināšanas platformas pašas pakalpojuma identitāti — kodā nav statisku akreditācijas datu, un tiešā klienta piekļuve ir liegta ar pašas datubāzes drošības noteikumiem. Dati ir šifrēti gan glabāšanā, gan pārraides laikā.

## 9. Izmaiņas

Mēs varam laiku pa laikam atjaunināt šo politiku. Būtiskas izmaiņas tiks atspoguļotas šeit, ar aktuālu datumu augšpusē.

---

**Jautājumi par saviem datiem?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Atpakaļ uz Palīdzības centru](index.html)
