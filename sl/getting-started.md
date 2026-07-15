---
title: IFG GEO Optimizer
description: Dokumentacija, pogosta vprašanja in pravne strani za Shopify aplikacijo IFG GEO Optimizer.
lang: sl
---

# Prvi koraki

<div class="lang-switcher">
{% include lang-switcher.html current="sl" slug="getting-started" %}
</div>

IFG GEO Optimizer ima devet področij, do katerih dostopate iz zgornje navigacije, ko je nastavitev zaključena: **Nadzorna plošča**, **Revizija kataloga**, **Crawler AI**, **Pogosta vprašanja izdelka**, **Link Coach**, **Vidnost AI**, **Cenik**, **Nastavitve** in **Podpora**. Ta vodič po vrsti razloži vsa področja, v vrstnem redu, v katerem jih večina trgovcev uporablja.

## 1. Namestitev in dokončanje čarovnika za nastavitev

Ob prvem odprtju kratek vodeni postopek nastavitve (približno 2 minuti) zbere osnovne podatke: jezik vmesnika, podrobnosti o vaši politiki vračil in dostave, podatke o vašem podjetju in — korak, ki je dejansko tehnično najpomembnejši — aktivacijo vgrajenega elementa aplikacije **GEO Schema** v urejevalniku teme. Nič od tega, kar aplikacija počne kasneje, ne doseže vaše spletne trgovine, dokler ta element ni aktiviran, zato ga je vredno ne preskočiti. Vse te odgovore lahko kadar koli spremenite kasneje v razdelku **Nastavitve**.

## 2. Nadzorna plošča

Vaša domača baza. Prikazuje vaš trenutni GEO rezultat (iz zadnje revizije), **matriko pripravljenosti** z osmimi signali na prvi pogled — izluščljivost vsebine, shema Organization, `llms.txt`, `agents.md`, dostop pajkov, pripravljenost MCP, povezljivost Link Coach in napotitveni promet iz AI — poleg prioritiziranega seznama "to popravi najprej" in števcev uporabe vašega paketa (generiranja pogostih vprašanj, velikost kataloga). Vse tukaj vodi neposredno na stran, kjer lahko ukrepate.

## 3. Revizija kataloga

Kliknite **Ponovno preglej katalog**, da preverite vsak izdelek glede na devet polj strukturiranih podatkov, ki jih iščejo iskalniki: slika, opis, znamka, SKU, GTIN, cena, tehnične specifikacije, politika vračil in politika dostave. Izdelki pod 80/100 prikažejo natanko, kaj manjka.

- **Popravek z enim klikom**: kjer lahko aplikacija varno izpelje manjkajoče podatke (običajno tehnične specifikacije iz obstoječih možnosti izdelka), boste videli gumb **Popravi**, ki jih zapiše neposredno v strukturirane podatke izdelka. Za polja, ki jih aplikacija ne more preveriti, se nič ne ugiba — na primer manjkajoča črtna koda ostane manjkajoča, namesto da bi bila izmišljena.
- **Ocena razčlenjevanja vsebine**: poleg preverjanja strukturiranih podatkov vsak izdelek dobi tudi ločeno oceno izluščljivosti — ne "ali je polje prisotno", temveč "ali lahko sistem AI/RAG iz tega opisa dejansko izlušči jasno dejstvo". Skopo, s pridevniki nabito besedilo doseže nižjo oceno, tudi če ima popolno oznako schema.org.
- **`llms.txt`**: generira resnično, s standardi skladno datoteko `llms.txt`, ki povzema vaš katalog za sisteme AI, postrežena na pravem korenu vaše trgovine (`/llms.txt`), ne skrita pod potjo App Proxy, kjer je pajki ne bi našli.
- **`agents.md`**: generira datoteko, ki opisuje vašo trgovino avtonomnim nakupovalnim agentom — različice, iskanje, blagajno — zgrajeno izključno iz resničnih podatkov, ki jih vaša trgovina že razkriva, brez izmišljanja.
- **Shema Organization**: objavi podatke o vašem podjetju (uradni naziv, ID za DDV/davčno številko, naslov) kot strukturirane podatke, tako da lahko sistemi AI preverijo, da ste resnično, odgovorno podjetje, preden vas priporočijo.

Pri paketu Free revizije zajemajo prvih 20 izdelkov, enkratno, brez zgodovine. Grow in Unlimited pregledata celoten katalog in ohranita vsak pretekli pregled za primerjavo trendov.

## 4. Crawler AI

Izberite izdelek in aplikacija pridobi njegovo stran natanko tako, kot to počne pajek AI — brez izvajanja JavaScripta, enako kot GPTBot, ClaudeBot ali PerplexityBot — tako da vidite natanko, kaj je vidno tem sistemom: ali jih vaš `robots.txt` blokira (preverjeno za vsak bot posebej, ne le splošno dovoli/zavrni), in ali vaši strukturirani podatki dejansko preživijo v surovi HTML kodi, ki jo ti boti berejo.

**Primerjava s konkurenco** (ločen zavihek na tej strani): prilepite URL izdelka konkurenta in dobite enake GEO signale, prikazane vzporedno z vašimi — enaka vrsta razlike, kot bi jo dobili z ročno revizijo, brez potrebe po prijavi v konkurentova lastna orodja.

## 5. Pogosta vprašanja izdelka

Pri paketu Grow ali Unlimited izberite izdelek in kliknite **Generiraj pogosta vprašanja** za tri do pet parov vprašanje-odgovor, sestavljenih izključno iz resničnega naslova, opisa, dobavitelja in specifikacij tega izdelka — model ima izrecno navodilo, naj nikoli ne doda podrobnosti, ki je ni že v vaših podatkih. Preglejte vsak osnutek; nič se ne objavi brez vaše izrecne **Odobritve**. Odobrena pogosta vprašanja se prikažejo na aktivni strani izdelka in so označena kot strukturirani podatki `FAQPage`, tako da so hkrati berljiva za ljudi in citirajoča za stroje.

**Preoblikovanje vsebine** (ločen zavihek na tej strani): aplikacija lahko preoblikuje opis izdelka, da postane gostejši s preverljivimi dejstvi in lažji za citiranje s strani generativnega sistema — vedno vidite primerjavo pred/po in odobrite, preden se karkoli zapiše nazaj v izdelek.

## 6. Link Coach

Analizira, kako dobro so vaši izdelki medsebojno povezani prek skupnih zbirk, dobaviteljev in oznak — notranje povezovanje je signal, ki ga sistemi AI uporabljajo za razumevanje, kaj vaš katalog pokriva kot celota, ne le ene strani naenkrat. Prikaže osamljene izdelke brez smiselnih povezav in razložljive predloge za to popraviti.

## 7. Vidnost AI

Dodajte do peščico pozivov, za katere realno pričakujete, da bi jih stranka postavila AI asistentu (omejitev je odvisna od vašega paketa — glejte Cenik spodaj), aplikacija pa vsak teden preveri, ali Claude, ChatGPT, Gemini in Perplexity omenjajo vašo trgovino v odgovoru, s sledenjem skozi čas za vsak sistem posebej. Pri paketih Grow in Unlimited to prikaže tudi, kako se primerjate z imenovanimi konkurenti pri istih pozivih.

**Napotitveni promet iz AI** (Grow in Unlimited): lahek piksel, ki spoštuje zasebnost, zazna, ko obisk spletne trgovine dejansko izvira iz enega od teh sistemov AI (prek referrerja, samo potem ko je obiskovalec podal privolitev za analitiko prek pasice s piškotki vaše trgovine), in poroča, koliko takih obiskov ste imeli v zadnjih 7 dneh — druga polovica kroga, ki je samo sledenje vidnosti ne more pokazati: ne le "ali smo omenjeni", temveč "ali ta omemba komu pošilja obiskovalce."

## 8. Podpora

Znotraj aplikacije (ikona spodaj desno) je na voljo klepetalni pomočnik AI za vprašanja o GEO, rezultatih vaše revizije ali delovanju posamezne funkcije. Če ne more pomagati, lahko zaprosite za pogovor s človekom, pogovor pa se posreduje neposredno podjetju IFG eCommerce.

## 9. Nastavitve

Tukaj upravljate odgovore čarovnika za nastavitev (politike, podatki o podjetju, jezik vmesnika — preklopite takoj med 30 jeziki, brez zamika pri nalaganju), ponovno preverite aktivacijo vgrajenega elementa teme in si ogledate obseg dovoljenj (scopes) Shopify vašega računa.

## 10. Cenik

**Cenik** prikazuje pakete Free, Grow in Unlimited vzporedno, mesečno ali letno (letno je pri obeh plačljivih paketih približno 2 meseca brezplačno). Kadar koli lahko nadgradite, znižate paket ali se vrnete na Free, neposredno iz aplikacije — brez potrebe po e-pošti. Za natančne omejitve paketov glejte [Pogosta vprašanja](faq.html).

To je celoten krog. Večina trgovcev znova zažene revizijo po dodajanju novih izdelkov, preveri simulator pajkov ob vsaki posodobitvi opisa in tedensko preleti matriko pripravljenosti na nadzorni plošči.

[← Nazaj v Center za pomoč](index.html)
