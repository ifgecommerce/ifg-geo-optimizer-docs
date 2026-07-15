---
title: IFG GEO Optimizer
description: Dokumentacija, česta pitanja i pravne stranice za Shopify aplikaciju IFG GEO Optimizer.
lang: hr
---

# Prvi koraci

<div class="lang-switcher">
{% include lang-switcher.html current="hr" slug="getting-started" %}
</div>

IFG GEO Optimizer ima devet područja, sva dostupna iz gornje navigacije nakon završetka postavljanja: **Dashboard**, **Audit kataloga**, **Crawler AI**, **FAQ proizvoda**, **Link Coach**, **Visibility AI**, **Cjenik**, **Postavke** i **Podrška**. Ovaj vodič prolazi kroz sve njih, redoslijedom kojim ih većina trgovaca koristi.

## 1. Instalacija i dovršetak čarobnjaka za postavljanje

Pri prvom otvaranju, kratko vođeno postavljanje (oko 2 minute) prikuplja osnovne podatke: jezik sučelja, detalje vaše politike povrata i dostave, podatke o vašoj tvrtki i — jedini korak koji je tehnički zaista bitan — aktivaciju app embeda **GEO Schema** u uredniku teme. Ništa od onoga što aplikacija radi nakon toga ne dopire do vaše trgovine dok ovaj embed nije uključen, stoga ga vrijedi ne preskočiti. Bilo koji od ovih odgovora možete kasnije promijeniti u **Postavkama**.

## 2. Dashboard

Vaša matična stranica. Prikazuje vaš trenutni GEO rezultat (iz posljednjeg audita), **Readiness Matrix** s osam signala na prvi pogled — ekstraktibilnost sadržaja, Organization schema, `llms.txt`, `agents.md`, pristup crawlerima, MCP spremnost, povezanost s Link Coachem i AI referral promet — plus prioritiziranu listu "ovo popravi prvo" i brojače korištenja vašeg plana (generiranja FAQ-a, veličina kataloga). Sve ovdje vodi izravno na stranicu na kojoj možete djelovati.

## 3. Audit kataloga

Kliknite **Ponovno skeniraj katalog** kako biste provjerili svaki proizvod prema devet polja strukturiranih podataka koje tražilice traže: slika, opis, brend, SKU, GTIN, cijena, tehničke specifikacije, politika povrata i politika dostave. Proizvodi ispod 80/100 pokazuju točno što nedostaje.

- **Ispravak jednim klikom**: gdje aplikacija sigurno može izvesti podatke koji nedostaju (obično tehničke specifikacije iz postojećih opcija proizvoda), vidjet ćete gumb **Ispravi** koji ih izravno upisuje u strukturirane podatke proizvoda. Ništa se ne pretpostavlja za polja koja aplikacija ne može provjeriti — nedostajući barkod, primjerice, ostaje nedostajući umjesto da se izmišlja.
- **Content chunking score**: uz provjeru strukturiranih podataka, svaki proizvod dobiva zaseban rezultat ekstraktibilnosti — ne "je li polje prisutno", nego "može li AI/RAG sustav zaista izvući čistu činjenicu iz ovog opisa". Oskudan, pridjevima nabijen tekst dobiva niži rezultat čak i uz savršen schema.org markup.
- **`llms.txt`**: generira pravi, standardima usklađen `llms.txt` koji sažima vaš katalog za AI sustave, poslužen na pravom korijenu vaše trgovine (`/llms.txt`), a ne skriven ispod putanje app proxyja gdje ga crawleri neće pronaći.
- **`agents.md`**: generira datoteku koja opisuje vašu trgovinu autonomnim kupovnim agentima — varijante, pretraživanje, checkout — izgrađenu isključivo od stvarnih podataka koje vaša trgovina već izlaže, ništa izmišljeno.
- **Organization schema**: objavljuje podatke vaše tvrtke (pravni naziv, OIB/PDV broj, adresu) kao strukturirane podatke, tako da AI motori mogu provjeriti da ste stvarna, odgovorna tvrtka prije nego što vas preporuče.

Na planu Free, auditi obuhvaćaju prvih 20 proizvoda, jednokratno, bez čuvanja povijesti. Grow i Unlimited skeniraju cijeli vaš katalog i čuvaju svaki prošli sken radi usporedbe trendova.

## 4. Crawler AI

Odaberite proizvod i aplikacija dohvaća njegovu stranicu točno onako kako to radi AI crawler — bez izvršavanja JavaScripta, isto kao GPTBot, ClaudeBot ili PerplexityBot — tako da vidite točno što je vidljivo ovim motorima: blokira li ih vaš `robots.txt` (provjereno po pojedinom botu, ne samo generičkim dopusti/zabrani), i preživljavaju li vaši strukturirani podaci zaista u sirovom HTML-u koji ovi botovi čitaju.

**Usporedba s konkurencijom** (zaseban tab na ovoj stranici): zalijepite URL proizvoda konkurenta i dobit ćete iste GEO signale uspoređene jedan pored drugog s vašima — ista vrsta razlike koju biste dobili ručnim auditom, bez potrebe za prijavom na alate samog konkurenta.

## 5. FAQ proizvoda

Na planu Grow ili Unlimited, odaberite proizvod i kliknite **Generiraj FAQ** za tri do pet parova pitanje-odgovor sastavljenih isključivo od stvarnog naziva, opisa, dobavljača i specifikacija tog proizvoda — model je izričito upućen da nikada ne doda detalj koji već nije u vašim podacima. Pregledajte svaki nacrt; ništa se ne objavljuje bez vašeg izričitog **Odobri**. Odobreni FAQ-ovi prikazuju se na uživo stranici proizvoda i označeni su kao `FAQPage` strukturirani podaci, tako da su čitljivi ljudima i citirajući strojevima.

**Prepisivanje sadržaja** (zaseban tab na ovoj stranici): aplikacija može prepisati opis proizvoda kako bi bio gušći provjerljivim činjenicama i lakši za citiranje generativnom motoru — uvijek vidite usporedbu prije/poslije i odobravate prije nego što se bilo što upiše natrag u proizvod.

## 6. Link Coach

Analizira koliko su vaši proizvodi dobro povezani jedni s drugima kroz zajedničke kolekcije, dobavljače i oznake — interno povezivanje signal je koji AI sustavi koriste kako bi razumjeli što vaš katalog obuhvaća u cjelini, ne samo jednu stranicu odjednom. Prikazuje proizvode bez smislenih veza i objašnjive prijedloge za rješavanje toga.

## 7. Visibility AI

Dodajte do nekoliko upita koje biste realno očekivali da kupac postavi AI asistentu (ograničenje ovisi o vašem planu — pogledajte Cjenik ispod), i svaki tjedan aplikacija provjerava spominju li Claude, ChatGPT, Gemini i Perplexity vašu trgovinu u odgovoru, praćeno kroz vrijeme po pojedinom motoru. Na planovima Grow i Unlimited, ovo također prikazuje kako se uspoređujete s imenovanim konkurentima na istim upitima.

**AI referral promet** (Grow i Unlimited): lagani piksel koji poštuje privatnost otkriva kada posjet trgovini zaista dolazi od jednog od ovih AI motora (putem referrera, samo nakon što je posjetitelj dao pristanak za analitiku putem bannera kolačića vaše trgovine) i izvještava koliko je takvih posjeta bilo u posljednjih 7 dana — druga polovica petlje koju samo praćenje vidljivosti ne može pokazati: ne samo "spominju li nas", nego "šalje li to spominjanje ikoga".

## 8. Podrška

AI chat asistent živi unutar aplikacije (ikona dolje desno) za pitanja o GEO-u, rezultatima vašeg audita ili kako funkcionira određena značajka. Ako ne može pomoći, možete zatražiti razgovor s čovjekom i razgovor se prosljeđuje izravno IFG eCommerceu.

## 9. Postavke

Ovdje upravljate odgovorima iz čarobnjaka za postavljanje (politike, podaci o tvrtki, jezik sučelja — prebacite se trenutno između 30 jezika, bez kašnjenja pri ponovnom učitavanju), ponovno provjeravate aktivaciju embeda teme i vidite Shopify opsege (scopes) vašeg računa.

## 10. Cjenik

**Cjenik** prikazuje Free, Grow i Unlimited jedan pored drugog, mjesečno ili godišnje (godišnje je otprilike 2 mjeseca besplatno na oba plaćena plana). U svakom trenutku možete nadograditi, downgradati ili se vratiti na Free, izravno iz aplikacije — bez potrebe za e-mailom. Pogledajte [Česta pitanja](faq.html) za točna ograničenja po planu.

To je cijela petlja. Većina trgovaca ponovno pokreće audit nakon dodavanja novih proizvoda, provjerava simulator crawlera kad god ažurira opis i tjedno baci pogled na Readiness Matrix na Dashboardu.

[← Natrag na Centar za pomoć](index.html)
