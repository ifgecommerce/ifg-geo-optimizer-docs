---
title: IFG GEO Optimizer
description: Documentație, întrebări frecvente și pagini legale pentru aplicația Shopify IFG GEO Optimizer.
lang: ro
---

# Primii pași

<div class="lang-switcher">
{% include lang-switcher.html current="ro" slug="getting-started" %}
</div>

IFG GEO Optimizer are nouă zone, toate accesibile din navigarea de sus odată ce configurarea este finalizată: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ produs**, **Link Coach**, **Visibility AI**, **Prețuri**, **Setări** și **Asistență**. Acest ghid parcurge toate aceste zone, în ordinea în care majoritatea comercianților le folosesc.

## 1. Instalează și finalizează asistentul de configurare

La prima deschidere, un scurt proces de configurare ghidată (aproximativ 2 minute) colectează elementele de bază: limba interfeței, detaliile politicii tale de retur și livrare, informațiile despre companie și — singurul pas care contează cu adevărat din punct de vedere tehnic — activarea embed-ului de aplicație **GEO Schema** în editorul temei tale. Nimic din ce face aplicația ulterior nu ajunge pe magazinul tău vitrină până când acest embed nu este activat, așa că merită să nu-l omiți. Poți schimba oricând aceste răspunsuri mai târziu din **Setări**.

## 2. Dashboard

Baza ta de start. Afișează scorul tău GEO curent (din ultimul audit), o **Matrice de pregătire** cu opt semnale dintr-o privire — extractibilitatea conținutului, schema Organization, `llms.txt`, `agents.md`, accesul crawler-elor, pregătirea pentru MCP, conectivitatea Link Coach și traficul de recomandare AI — plus o listă prioritizată „rezolvă asta mai întâi" și contoarele de utilizare ale planului tău (generări FAQ, dimensiunea catalogului). Totul aici duce direct la pagina unde poți acționa.

## 3. Audit catalog

Apasă **Rescanează catalogul** pentru a verifica fiecare produs în raport cu nouă câmpuri de date structurate căutate de motoarele de căutare: imagine, descriere, brand, SKU, GTIN, preț, specificații tehnice, politică de retur și politică de livrare. Produsele sub 80/100 arată exact ce lipsește.

- **Remediere cu un clic**: acolo unde aplicația poate deriva în siguranță datele lipsă (de obicei specificații tehnice din opțiunile existente ale produsului), vei vedea un buton **Remediază** care le scrie direct în datele structurate ale produsului. Nimic nu este ghicit pentru câmpurile pe care aplicația nu le poate verifica — de exemplu, un cod de bare lipsă rămâne lipsă în loc să fie inventat.
- **Scor de content chunking**: pe lângă verificarea datelor structurate, fiecare produs primește un scor separat de extractibilitate — nu „este câmpul prezent", ci „poate un sistem AI/RAG să extragă efectiv un fapt clar din această descriere". Un text sărac, plin de adjective, obține un scor mai mic chiar și cu un markup schema.org perfect.
- **`llms.txt`**: generează un fișier `llms.txt` real, conform standardelor, care rezumă catalogul tău pentru sistemele AI, servit la rădăcina reală a magazinului tău (`/llms.txt`), nu ascuns sub o cale de app proxy unde crawler-ele nu-l vor găsi.
- **`agents.md`**: generează un fișier care descrie magazinul tău pentru agenții de cumpărături autonomi — variante, căutare, checkout — construit doar din date reale pe care magazinul tău le expune deja, nimic inventat.
- **Schema Organization**: publică detaliile companiei tale (denumire legală, CUI/cod fiscal, adresă) ca date structurate, astfel încât motoarele AI să poată verifica faptul că ești o afacere reală și responsabilă înainte de a te recomanda.

În planul Free, auditurile acoperă primele 20 de produse, o singură dată, fără istoric păstrat. Grow și Unlimited scanează întregul catalog și păstrează fiecare scanare anterioară pentru comparație de tendințe.

## 4. Crawler AI

Alege un produs, iar aplicația îi preia pagina exact așa cum face un crawler AI — fără execuție JavaScript, la fel ca GPTBot, ClaudeBot sau PerplexityBot — astfel încât vezi exact ce este vizibil pentru aceste motoare: dacă `robots.txt`-ul tău le blochează (verificat per bot, nu doar un allow/deny generic) și dacă datele tale structurate supraviețuiesc cu adevărat în HTML-ul brut citit de acești boți.

**Comparație cu concurența** (tab separat pe această pagină): lipește URL-ul unui produs concurent și obții aceleași semnale GEO comparate direct cu ale tale — aceeași diferență de fond pe care ai obține-o dintr-un audit manual, fără a fi nevoie să te înscrii la propriile instrumente ale concurentului.

## 5. FAQ produs

Pe Grow sau Unlimited, alege un produs și apasă **Generează FAQ** pentru trei până la cinci perechi întrebare-răspuns redactate doar din titlul, descrierea, furnizorul și specificațiile reale ale acelui produs — modelului i se cere explicit să nu adauge niciodată un detaliu care nu este deja în datele tale. Revizuiește fiecare ciornă; nimic nu se publică fără **Aprobarea** ta explicită. FAQ-urile aprobate apar pe pagina live a produsului și sunt marcate ca date structurate `FAQPage`, astfel încât sunt atât lizibile de oameni, cât și citabile de mașini.

**Rescriere conținut** (tab separat pe această pagină): aplicația poate rescrie o descriere de produs pentru a fi mai densă în fapte verificabile și mai ușor de citat de un motor generativ — vezi întotdeauna o comparație înainte/după și aprobi înainte ca ceva să fie scris înapoi în produs.

## 6. Link Coach

Analizează cât de bine sunt conectate produsele tale între ele prin colecții, furnizori și etichete comune — legăturile interne sunt un semnal pe care sistemele AI îl folosesc pentru a înțelege ce acoperă catalogul tău în ansamblu, nu doar o singură pagină odată. Arată produsele orfane fără conexiuni semnificative și sugestii explicabile pentru a remedia asta.

## 7. Visibility AI

Adaugă până la câteva prompt-uri pe care te-ai aștepta în mod realist ca un client să le adreseze unui asistent AI (limita depinde de planul tău — vezi Prețuri mai jos), iar în fiecare săptămână aplicația verifică dacă Claude, ChatGPT, Gemini și Perplexity menționează magazinul tău în răspuns, urmărit în timp per motor. Pe Grow și Unlimited, aceasta arată și cum te compari cu concurenți numiți pe aceleași prompt-uri.

**Trafic de recomandare AI** (Grow și Unlimited): un pixel ușor, care respectă confidențialitatea, detectează când o vizită pe magazinul vitrină provine efectiv de la unul dintre aceste motoare AI (prin referrer, doar după ce vizitatorul a acordat consimțământul de analiză prin bannerul de cookie-uri al magazinului tău) și raportează câte astfel de vizite ai avut în ultimele 7 zile — a doua jumătate a buclei pe care urmărirea vizibilității singură nu o poate arăta: nu doar „suntem menționați", ci „acea mențiune trimite pe cineva".

## 8. Asistență

Un asistent de chat AI trăiește în aplicație (pictograma din dreapta jos) pentru întrebări despre GEO, rezultatele auditului tău sau modul în care funcționează o anumită funcționalitate. Dacă nu te poate ajuta, poți cere să vorbești cu un om, iar conversația este redirecționată direct către IFG eCommerce.

## 9. Setări

Aici gestionezi răspunsurile din asistentul de configurare (politici, date companie, limba interfeței — comută instantaneu între 30 de limbi, fără întârziere la reîncărcare), reverifici activarea embed-ului temei și vezi permisiunile (scopes) Shopify ale contului tău.

## 10. Prețuri

**Prețuri** afișează Free, Grow și Unlimited alături, lunar sau anual (anual este aproximativ 2 luni gratuite pe ambele niveluri plătite). Poți face upgrade, downgrade sau reveni la Free oricând, direct din aplicație — fără a fi nevoie de email. Vezi [Întrebările frecvente](faq.html) pentru limitele exacte ale planurilor.

Aceasta este bucla completă. Majoritatea comercianților rulează din nou un audit după adăugarea de produse noi, verifică simulatorul de crawler ori de câte ori actualizează o descriere și aruncă o privire săptămânal la Matricea de pregătire din Dashboard.

[← Înapoi la Centrul de asistență](index.html)
