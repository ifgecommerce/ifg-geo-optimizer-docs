---
title: IFG GEO Optimizer
description: Shopify rakenduse IFG GEO Optimizer dokumentatsioon, KKK ja õiguslikud leheküljed.
lang: et
---

# Alustamine

<div class="lang-switcher">
{% include lang-switcher.html current="et" slug="getting-started" %}
</div>

IFG GEO Optimizeril on üheksa valdkonda, kõik kättesaadavad ülemisest navigatsioonist pärast seadistamise lõpetamist: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** ja **Support**. See juhend käib need kõik läbi, järjekorras, mida enamik kauplejaid kasutab.

## 1. Paigalda ja lõpeta seadistuse viisard

Esimesel avamisel kogub lühike juhendatud seadistus (umbes 2 minutit) põhiandmed: liidese keel, sinu tagastus- ja tarnepoliitika andmed, ettevõtte info ning — samm, mis tehniliselt tegelikult loeb — **GEO Schema** rakenduse manuse aktiveerimine sinu teema redaktoris. Miski, mida rakendus hiljem teeb, ei jõua sinu e-poe vaateni enne, kui see manus on sisse lülitatud, seega tasub seda sammu mitte vahele jätta. Kõiki neid vastuseid saad hiljem alati muuta **Settings** alt.

## 2. Dashboard

Sinu kodubaas. See näitab sinu praegust GEO skoori (viimasest auditist), **Readiness Matrix** kaheksa kiirülevaate signaaliga — sisu eraldatavus, Organization skeem, `llms.txt`, `agents.md`, crawleri ligipääs, MCP valmisolek, Link Coachi ühenduvus ja AI-suunatud liiklus — pluss prioritiseeritud "paranda see esimesena" nimekiri ja sinu paketi kasutusnäidikud (KKK genereerimised, kataloogi suurus). Kõik siin viitab otse lehele, kus saad selle kallal toimetada.

## 3. Audit catalog

Klõpsa **Rescan catalog**, et kontrollida iga toodet üheksa struktureeritud andmete välja suhtes, mida otsingumootorid otsivad: pilt, kirjeldus, kaubamärk, SKU, GTIN, hind, tehnilised andmed, tagastuspoliitika ja tarnepoliitika. Alla 80/100 punkti tooted näitavad täpselt, mis puudub.

- **Ühe klõpsuga parandus**: kus rakendus saab puuduvad andmed turvaliselt tuletada (tavaliselt tehnilised andmed sinu olemasolevatest tootevalikutest), näed **Fix** nuppu, mis kirjutab need otse toote struktureeritud andmetesse. Väljade puhul, mida rakendus ei saa kontrollida, ei arvata midagi — näiteks puuduv triipkood jääb puuduvaks, selle asemel et see välja mõelda.
- **Sisu tükeldamise (chunking) skoor**: koos struktureeritud andmete kontrolliga saab iga toode eraldi eraldatavuse skoori — mitte "kas väli on olemas", vaid "kas AI/RAG süsteem suudab sellest kirjeldusest tegelikult puhta fakti kätte saada". Õhuke, omadussõnarohke tekst saab madalama skoori isegi täiusliku schema.org märgistuse korral.
- **`llms.txt`**: genereerib tõelise, standarditele vastava `llms.txt` faili, mis võtab sinu kataloogi AI süsteemide jaoks kokku ja mida serveeritakse sinu poe tegelikust juurest (`/llms.txt`), mitte peidetuna rakenduse proksi tee alla, kust crawlerid seda ei leia.
- **`agents.md`**: genereerib faili, mis kirjeldab sinu poodi autonoomsetele ostuagentidele — variandid, otsing, kassa — üles ehitatud ainult sinu poe juba avalikustatud päris andmete põhjal, ilma väljamõeldisteta.
- **Organization skeem**: avaldab sinu ettevõtte andmed (juriidiline nimi, käibemaksu-/maksukohustuslase number, aadress) struktureeritud andmetena, et AI mootorid saaksid enne sinu soovitamist kontrollida, et oled päris, vastutustundlik ettevõte.

Free paketis katab audit sinu esimest 20 toodet, ühekordselt, ilma ajaloota. Grow ja Unlimited skaneerivad kogu sinu kataloogi ja säilitavad iga eelmise skaneerimise trendide võrdlemiseks.

## 4. Crawler AI

Vali toode ja rakendus toob selle lehe täpselt nii, nagu AI crawler seda teeb — ilma JavaScripti käivitamiseta, samamoodi nagu GPTBot, ClaudeBot või PerplexityBot — nii et näed täpselt, mis on nendele mootoritele nähtav: kas sinu `robots.txt` blokeerib neid (kontrollitud boti kaupa, mitte lihtsalt üldine luba/keeld), ja kas sinu struktureeritud andmed tegelikult säilivad toorest HTML-ist, mida need botid loevad.

**Konkurendi võrdlus** (oma vahekaart sellel lehel): kleebi konkurendi tootelehe URL ja saad samad GEO signaalid kõrvuti sinu omadega võrreldud — samasugune erinevus, mida saaksid käsitsi auditist, ilma vajaduseta konkurendi enda tööriistadesse registreeruda.

## 5. FAQ product

Grow või Unlimited paketis vali toode ja klõpsa **Generate FAQs**, et saada kolm kuni viis küsimuse-vastuse paari, mis on koostatud ainult selle toote päris pealkirja, kirjelduse, tootja ja tehniliste andmete põhjal — mudelile on selgesõnaliselt öeldud, et ta ei tohi kunagi lisada detaili, mida sinu andmetes juba pole. Vaata iga mustand üle; miski ei avaldata ilma sinu selgesõnalise **Approve** kinnituseta. Heaks kiidetud KKK-d ilmuvad tootelehele ja on märgistatud `FAQPage` struktureeritud andmetena, seega on need korraga nii inimesele loetavad kui masinale tsiteeritavad.

**Sisu ümberkirjutamine** (oma vahekaart sellel lehel): rakendus saab kirjutada toote kirjelduse ümber tihedamaks kontrollitavatest faktidest ja lihtsamaks tsiteerida generatiivsele mootorile — näed alati enne/pärast võrdlust ja kinnitad enne, kui midagi tootele tagasi kirjutatakse.

## 6. Link Coach

Analüüsib, kui hästi on sinu tooted omavahel ühendatud jagatud kollektsioonide, tootjate ja siltide kaudu — sisemine lingistruktuur on signaal, mida AI süsteemid kasutavad, et mõista, mida sinu kataloog tervikuna katab, mitte ainult ühte lehte korraga. Näitab orbtooteid ilma sisuliste ühendusteta ja selgitatud soovitusi selle parandamiseks.

## 7. Visibility AI

Lisa kuni käputäis päringuid, mida sa realistlikult ootaksid kliendilt AI assistendile küsimist (limiit sõltub sinu paketist — vaata Pricing allpool), ja iga nädal kontrollib rakendus, kas Claude, ChatGPT, Gemini ja Perplexity mainivad sinu poodi vastuses, jälgituna aja jooksul mootori kaupa. Grow ja Unlimited paketis näitab see ka, kuidas sa võrdled nimetatud konkurentidega samadel päringutel.

**AI-suunatud liiklus** (Grow ja Unlimited): kerge, privaatsust austav pikslikood tuvastab, kui poe külastus tuleb tegelikult ühest neist AI mootoritest (viitaja kaudu, ainult pärast seda, kui külastaja on andnud analüütika nõusoleku sinu poe küpsisebänneri kaudu) ja raporteerib, mitu sellist külastust said viimase 7 päeva jooksul — teine pool tsüklist, mida ainuüksi nähtavuse jälgimine ei saa näidata: mitte ainult "kas meid mainitakse", vaid "kas see mainimine saadab kellegi meile".

## 8. Support

AI vestlusassistent elab rakenduses (alumine parem nurk ikoon) küsimuste jaoks GEO kohta, sinu auditi tulemuste kohta või selle kohta, kuidas mingi funktsioon töötab. Kui see ei saa aidata, võid küsida inimesega rääkimist ja vestlus edastatakse otse IFG eCommerce'ile.

## 9. Settings

Kus haldad seadistuse viisardi vastuseid (poliitikad, ettevõtte andmed, liidese keel — vaheta koheselt 30 keele vahel, ilma laadimisviivituseta), kontrollid uuesti teema manuse aktiveerimist ja näed oma konto Shopify õigusi (scope).

## 10. Pricing

**Pricing** näitab Free, Grow ja Unlimited pakette kõrvuti, kuu- või aastapõhiselt (aastapõhine on mõlemal tasulisel paketil ligikaudu 2 kuud tasuta). Saad igal ajal uuendada, alandada või tühistada tagasi Free peale, otse rakendusest — ilma e-kirjata. Vaata [KKK](faq.html) täpsete paketilimiitide jaoks.

See ongi kogu tsükkel. Enamik kauplejaid käivitab auditi uuesti pärast uute toodete lisamist, kontrollib crawleri simulaatorit iga kord, kui uuendab kirjeldust, ja heidab pilgu Dashboardi Readiness Matrixile iganädalaselt.

[← Tagasi Abikeskusesse](index.html)
