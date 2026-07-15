---
title: IFG GEO Optimizer
description: Dokumentācija, BUJ un juridiskās lapas Shopify lietotnei IFG GEO Optimizer.
lang: lv
---

# Darba sākšana

<div class="lang-switcher">
{% include lang-switcher.html current="lv" slug="getting-started" %}
</div>

IFG GEO Optimizer sastāv no deviņām sadaļām, kas pēc iestatīšanas visas pieejamas no augšējās navigācijas: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** un **Support**. Šis ceļvedis apraksta visas sadaļas secībā, kādā tās parasti izmanto tirgotāji.

## 1. Instalē un pabeidz iestatīšanas vedni

Pirmajā atvēršanas reizē īss vadītais iestatījums (apmēram 2 minūtes) apkopo pamatinformāciju: saskarnes valodu, tavas atgriešanas un piegādes politikas detaļas, uzņēmuma informāciju un — vienīgo soli, kam tehniski patiešām ir nozīme — **GEO Schema** app embed aktivizēšanu tēmas redaktorā. Nekas no tā, ko lietotne dara pēc tam, nesasniedz tavu veikala vitrīnu, kamēr šis embed nav ieslēgts, tāpēc šo soli nevajadzētu izlaist. Jebkuru no šīm atbildēm vēlāk vienmēr var mainīt sadaļā **Settings**.

## 2. Dashboard

Tava sākuma bāze. Tā parāda tavu pašreizējo GEO rezultātu (no pēdējā audita), **Readiness Matrix** ar astoņiem signāliem vienā skatā — satura izvelkamību (content extractability), Organization schema, `llms.txt`, `agents.md`, crawler piekļuvi, MCP gatavību, Link Coach savienojamību un AI ieteikto apmeklējumu plūsmu —, kā arī prioritizētu "labo šo vispirms" sarakstu un tava plāna izmantošanas skaitītājus (FAQ ģenerēšanas, kataloga izmērs). Viss šeit ved tieši uz lapu, kurā vari rīkoties.

## 3. Audit catalog

Klikšķini **Rescan catalog**, lai pārbaudītu katru produktu pret deviņiem strukturēto datu laukiem, ko meklē meklētājprogrammas: attēls, apraksts, zīmols, SKU, GTIN, cena, tehniskās specifikācijas, atgriešanas politika un piegādes politika. Produkti zem 80/100 parāda tieši to, kas trūkst.

- **Viena klikšķa labojums**: ja lietotne var droši atvasināt trūkstošos datus (parasti tehniskās specifikācijas no esošajām produkta opcijām), redzēsi pogu **Fix**, kas tos ieraksta tieši produkta strukturētajos datos. Nekas netiek uzminēts laukiem, ko lietotne nevar pārbaudīt — piemēram, trūkstošs svītrkods paliek trūkstošs, nevis tiek izdomāts.
- **Content chunking score**: līdzās strukturēto datu pārbaudei katrs produkts saņem atsevišķu izvelkamības rezultātu — nevis "vai lauks ir klāt", bet "vai AI/RAG sistēma no šī apraksta patiešām var izvilkt tīru faktu". Trūcīgs, ar īpašības vārdiem pārblīvēts teksts saņem zemāku rezultātu pat ar nevainojamu schema.org marķējumu.
- **`llms.txt`**: ģenerē reālu, standartiem atbilstošu `llms.txt` failu, kas apkopo tavu katalogu AI sistēmām, un to apkalpo tava veikala patiesajā saknē (`/llms.txt`), nevis apraktu zem app proxy ceļa, kur crawleri to neatradīs.
- **`agents.md`**: ģenerē failu, kas apraksta tavu veikalu autonomiem iepirkšanās aģentiem — variantus, meklēšanu, norēķināšanos — un ir veidots tikai no reāliem datiem, ko tavs veikals jau publisko, neko neizdomājot.
- **Organization schema**: publicē tava uzņēmuma datus (juridisko nosaukumu, PVN/nodokļu numuru, adresi) kā strukturētus datus, lai AI dzinēji var pārbaudīt, ka esi reāls, atbildīgs uzņēmums, pirms tevi iesaka.

Free plānā audits aptver pirmos 20 produktus, vienreizēji, bez vēstures saglabāšanas. Grow un Unlimited skenē visu katalogu un saglabā katru iepriekšējo skenējumu tendenču salīdzināšanai.

## 4. Crawler AI

Izvēlies produktu, un lietotne ielādē tā lapu tieši tā, kā to dara AI crawler — bez JavaScript izpildes, tāpat kā GPTBot, ClaudeBot vai PerplexityBot — tā tu redzi precīzi to, kas šiem dzinējiem ir redzams: vai tavs `robots.txt` tos bloķē (pārbaudīts katram robotam atsevišķi, nevis tikai vispārīgs atļauts/liegts), un vai tavi strukturētie dati patiešām saglabājas neapstrādātajā HTML, ko šie roboti lasa.

**Konkurentu salīdzinājums** (atsevišķa cilne šajā lapā): ielīmē konkurenta produkta URL un saņem tos pašus GEO signālus blakus salīdzinātus ar saviem — tāda pati atšķirība pēc būtības, kādu iegūtu manuālā audita rezultātā, bez nepieciešamības reģistrēties konkurenta pašu rīkos.

## 5. FAQ product

Grow vai Unlimited plānā izvēlies produktu un klikšķini **Generate FAQs**, lai iegūtu trīs līdz piecus jautājumu-atbilžu pārus, kas veidoti tikai no šī produkta reālā nosaukuma, apraksta, ražotāja un specifikācijām — modelim ir tieši norādīts nekad nepievienot detaļu, kuras jau nav tavos datos. Pārskati katru melnrakstu; nekas netiek publicēts bez tava skaidra **Approve**. Apstiprinātie FAQ parādās aktīvajā produkta lapā un ir marķēti kā `FAQPage` strukturētie dati, tāpēc tie ir gan cilvēkiem lasāmi, gan mašīnām citējami.

**Satura pārrakstīšana** (atsevišķa cilne šajā lapā): lietotne var pārrakstīt produkta aprakstu, lai tas būtu blīvāks ar pārbaudāmiem faktiem un vieglāk citējams ģeneratīvajam dzinējam — vienmēr redzi salīdzinājumu "pirms/pēc" un apstiprini, pirms kaut kas tiek ierakstīts atpakaļ produktā.

## 6. Link Coach

Analizē, cik labi tavi produkti ir savstarpēji savienoti caur kopīgām kolekcijām, ražotājiem un tagiem — iekšējā savienošana ir signāls, ko AI sistēmas izmanto, lai saprastu, ko tavs katalogs aptver kopumā, nevis tikai vienu lapu vienlaikus. Parāda produktus bez jēgpilniem savienojumiem un izskaidrojamus ieteikumus, kā to labot.

## 7. Visibility AI

Pievieno līdz pat pāris uzvednēm (prompts), ko reāli sagaidītu, ka klients uzdotu AI asistentam (limits atkarīgs no tava plāna — skati Pricing zemāk), un katru nedēļu lietotne pārbauda, vai Claude, ChatGPT, Gemini un Perplexity piemin tavu veikalu atbildē, izsekojot to laika gaitā katram dzinējam atsevišķi. Grow un Unlimited plānos tas parāda arī, kā tu salīdzinies ar nosauktiem konkurentiem uz tām pašām uzvednēm.

**AI ieteiktais apmeklējums** (Grow un Unlimited): viegls, privātumu respektējošs pikselis nosaka, kad veikala apmeklējums patiešām nāk no viena no šiem AI dzinējiem (caur referrer, tikai pēc tam, kad apmeklētājs devis analītikas piekrišanu caur tava veikala sīkdatņu joslu) un ziņo, cik daudz šādu apmeklējumu bijis pēdējās 7 dienās — otrā puse cilpai, ko pati visibility tracking nevar parādīt: ne tikai "vai mūs piemin", bet "vai šis pieminējums kādu atsūta".

## 8. Support

Lietotnē (apakšējā labajā stūrī ikona) darbojas AI tērzēšanas asistents jautājumiem par GEO, tava audita rezultātiem vai to, kā darbojas konkrēta funkcija. Ja tas nevar palīdzēt, vari lūgt runāt ar cilvēku, un saruna tiek pārsūtīta tieši uz IFG eCommerce.

## 9. Settings

Šeit pārvaldi iestatīšanas vedņa atbildes (politikas, uzņēmuma datus, saskarnes valodu — pārslēdz uzreiz starp 30 valodām, bez pārlādes aizkaves), atkārtoti pārbaudi tēmas embed aktivizāciju un redzi sava konta Shopify piekļuves tiesības (scopes).

## 10. Pricing

**Pricing** parāda Free, Grow un Unlimited blakus, mēneša vai gada abonementā (gada abonements ir aptuveni 2 mēneši bez maksas abos maksas plānos). Vari jebkurā brīdī paaugstināt, pazemināt plānu vai atcelt atpakaļ uz Free tieši lietotnē — bez e-pasta nepieciešamības. Skati [BUJ](faq.html) precīzus plāna limitus.

Tas ir viss cikls. Lielākā daļa tirgotāju atkārtoti palaiž auditu pēc jaunu produktu pievienošanas, pārbauda crawler simulatoru ikreiz, kad atjaunina aprakstu, un ik nedēļu paskatās uz Dashboard Readiness Matrix.

[← Atpakaļ uz Palīdzības centru](index.html)
