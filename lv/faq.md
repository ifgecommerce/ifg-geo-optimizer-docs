---
title: IFG GEO Optimizer
description: Dokumentācija, BUJ un juridiskās lapas Shopify lietotnei IFG GEO Optimizer.
lang: lv
---

# Biežāk uzdotie jautājumi

<div class="lang-switcher">
{% include lang-switcher.html current="lv" slug="faq" %}
</div>

**Kāda ir atšķirība starp GEO un SEO?**
Tradicionālais SEO optimizē meklētājprogrammām, kas sarindo un uzskaita saites. GEO (Generative Engine Optimization) optimizē AI sistēmām, kas lasa tavu saturu un tieši ģenerē atbildi vai ieteikumu — ChatGPT, Perplexity, Gemini, Claude un Google AI Overviews. Abi pārklājas, taču GEO pievērš uzmanību lietām, ko klasiskie SEO rīki nepārbauda: vai tavai produkta lapai ir pilnīgi strukturētie dati, vai AI crawler patiešām var nolasīt tavu saturu bez JavaScript izpildes, un vai tavs teksts ir uzrakstīts tā, lai to būtu viegli citēt.

**Vai lietotne jebkad piekļūst manu klientu datiem?**
Nē, personiskus klientu datus nē. Lietotnes Shopify atļaujas ir `read_products`, `write_products`, `read_themes` un `write_pixels` — tavu katalogu lasa un uzlabo, pārbauda, vai tēmas embed ir aktīvs, un aktivizē anonīmu veikala apmeklējumu pikseli (skati zemāk). Tā nekad nepieprasa pasūtījumus vai klientu ierakstus. Pilnu izklāstu skati [Privātuma politikā](privacy.html).

**Kas ir AI ieteiktā apmeklējuma pikselis, un vai tas izseko manus klientus?**
Visos plānos neliels Web Pixel nosaka, kad veikala apmeklējums nāk no zināma AI dzinēja (caur pārlūka referrer) un ziņo dzinēju, lapu un laika zīmogu — neko, kas identificētu apmeklētāju, bez sīkdatnēm, bez sesijas datiem. Tas darbojas tikai tad, ja apmeklētājs jau devis analītikas piekrišanu caur tava veikala sīkdatņu joslu (Shopify Customer Privacy API). Tas tiek izmantots, lai parādītu Dashboard bloku ("AI ieteiktais apmeklējums, pēdējās 7 dienas") — Visibility AI izsekošanas pretinieks, kas pasaka, vai tevi piemin, bet ne vai šis pieminējums kādu atsūta.

**Ko tieši maina poga "Fix" kataloga auditā?**
Tā ieraksta trūkstošos schema.org strukturētos datus produkta metalauku (metafield) — tādas lietas kā tehniskās specifikācijas, kas atvasinātas no tavām esošajām produkta opcijām. Tā nekad nemaina produkta nosaukumu, aprakstu, attēlus vai cenu, un nekad neizdomā datus, kurus nevar pārbaudīt: piemēram, trūkstošs svītrkods paliek trūkstošs, nevis tiek uzminēts.

**Vai FAQ atbildes un pārrakstītie apraksti ir AI izdomāti, vai balstīti uz manu reālo produktu?**
Modelis redz tikai tos produkta datus, kas tev jau ir — nosaukumu, aprakstu, ražotāju un tehniskās specifikācijas —, un tam ir tieši norādīts nepievienot neko, kā šajos datos nav. Tu pārskati katru FAQ vai pārrakstīto aprakstu pirms publicēšanas; nekas netiek automātiski padarīts aktīvs.

**Kas notiek ar maniem datiem, ja atinstalēju lietotni?**
Tava veikala konfigurācija, saglabātie audits, FAQ un satura pārrakstīšanas melnraksti, visibility uzvednes un AI ieteiktā apmeklējuma notikumi tiek automātiski dzēsti, kad Shopify mums paziņo par atinstalēšanu. Lietotne pēc tavas aiziešanas neko nepatur.

**Vai varu atcelt vai pazemināt plānu, nesazinoties ar atbalstu?**
Jā. Dodies uz **Pricing** lietotnē un jebkurā brīdī pārslēdzies uz Free — tas stājas spēkā nekavējoties, e-pasts nav nepieciešams.

## Plāna limiti

| Funkcija | Free | Grow | Unlimited |
|---|---|---|---|
| Kataloga audits | Pirmie 20 produkti, vienreizēji, bez vēstures | Pilns katalogs + vēsture | Pilns katalogs + vēsture |
| Crawler simulator | 20/mēnesī | 300/mēnesī | 1000/mēnesī |
| Konkurentu salīdzinājums | 10/mēnesī | 50/mēnesī | 150/mēnesī |
| FAQ ģenerēšana | Nav iekļauts | 500/mēnesī | 500/mēnesī |
| Satura pārrakstīšana | Nav iekļauts | 300/mēnesī | 300/mēnesī |
| Visibility AI (izsekotās uzvednes) | Nav iekļauts | 5 uzvednes | 15 uzvednes |
| AI ieteiktā apmeklējuma pikselis | Iekļauts | Iekļauts | Iekļauts |
| AI atbalsta tērzēšana | 1000 ziņu/mēnesī | 1000 ziņu/mēnesī | 1000 ziņu/mēnesī |
| Saskarnes valodas | Visas 30 | Visas 30 | Visas 30 |

Mēneša cena: Free $0, Grow $9.99, Unlimited $19.99. Gada abonements Grow/Unlimited plānos ir aptuveni divi mēneši bez maksas, salīdzinot ar mēneša apmaksu.

**Kāpēc Free plāns aptver tikai 20 produktus?**
Tas ļauj redzēt reālus rezultātus savā katalogā, pirms izvēlies maksas plānu. Grow un Unlimited noņem šo ierobežojumu un saglabā pilnu iepriekšējo audits vēsturi.

**Vai FAQ ģenerēšanai patiešām ir limits pat Unlimited plānā?**
Jā — 500 ģenerācijas mēnesī, apzināti, pat augstākajā plānā. Tas nodrošina funkcijas ilgtspēju pie pašreizējās cenas; ja tev ir liela apjoma katalogs, kam vajag vairāk, sazinies ar mums, un mēs kaut ko atrisināsim.

**Kāpēc AI atbalsta tērzēšana ir vienāda visos plānos?**
Tas ir produkta lēmums, nevis izlaidums: atbalsts ir iekļauts visiem, nekad kā maksas atšķirība. Ziņu limits (1000/mēnesī) pastāv tikai kā tehnisks aizsargs pret ļaunprātīgu izmantošanu, nevis kā reāls ierobežojums — neviena likumīga izmantošana tam pat tuvu nenonāk.

**Atradu kļūdu vai kaut kas izskatās nepareizi. Kam pateikt?**
Raksti uz [info@ifgecommerce.com](mailto:info@ifgecommerce.com), aprakstot, ko redzēji, un, ja iespējams, kuru produktu vai lapu — parasti ar to pietiek, lai ātri to izsekotu. Vari izmantot arī AI atbalsta tērzēšanu lietotnē un palūgt runāt ar cilvēku.

[← Atpakaļ uz Palīdzības centru](index.html)
