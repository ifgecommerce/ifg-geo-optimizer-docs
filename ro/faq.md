---
title: IFG GEO Optimizer
description: Documentație, întrebări frecvente și pagini legale pentru aplicația Shopify IFG GEO Optimizer.
lang: ro
---

# Întrebări frecvente

<div class="lang-switcher">
{% include lang-switcher.html current="ro" slug="faq" %}
</div>

**Care este diferența dintre GEO și SEO?**
SEO tradițional optimizează pentru motoare de căutare care clasează și listează linkuri. GEO (Generative Engine Optimization) optimizează pentru sistemele AI care citesc conținutul tău și generează direct un răspuns sau o recomandare — ChatGPT, Perplexity, Gemini, Claude și Google AI Overviews. Cele două se suprapun, dar GEO se ocupă de lucruri pe care instrumentele SEO clasice nu le verifică: dacă pagina ta de produs are date structurate complete, dacă un crawler AI poate citi efectiv conținutul tău fără a executa JavaScript și dacă textul tău este scris într-un mod ușor de citat.

**Aplicația atinge vreodată datele clienților mei?**
Nu, niciun fel de date personale ale clienților. Permisiunile Shopify ale aplicației sunt `read_products`, `write_products`, `read_themes` și `write_pixels` — citirea și îmbunătățirea catalogului tău, verificarea că embed-ul temei este activ și activarea unui pixel anonim de trafic pe magazinul vitrină (vezi mai jos). Nu solicită niciodată comenzi sau înregistrări ale clienților. Vezi [Politica de confidențialitate](privacy.html) pentru detalii complete.

**Ce este pixelul de trafic de recomandare AI și îmi urmărește clienții?**
Pe Grow și Unlimited, un mic Web Pixel detectează când o vizită pe magazinul vitrină ajunge de la un motor AI cunoscut (prin referrer-ul browserului) și raportează motorul, pagina și o marcă temporală — nimic care să identifice vizitatorul, fără cookie-uri, fără date de sesiune. Rulează doar dacă vizitatorul a acordat deja consimțământul de analiză prin bannerul de cookie-uri al magazinului tău (Customer Privacy API de la Shopify). Este folosit pentru a afișa o casetă în Dashboard („Trafic de recomandare AI, ultimele 7 zile") — completarea urmăririi Visibility AI, care îți spune dacă ești menționat, dar nu și dacă acea mențiune a trimis pe cineva.

**Ce modifică efectiv butonul „Remediază" din auditul de catalog?**
Scrie datele structurate schema.org lipsă într-un metafield al produsului — lucruri precum specificații tehnice derivate din opțiunile existente ale produsului. Nu atinge niciodată titlul, descrierea, imaginile sau prețul produsului tău și nu inventează niciodată date pe care nu le poate verifica: de exemplu, un cod de bare lipsă rămâne lipsă în loc să fie ghicit.

**Răspunsurile FAQ și descrierile rescrise sunt inventate de AI sau se bazează pe produsul meu real?**
Modelul vede doar datele de produs pe care le ai deja — titlu, descriere, furnizor și specificații tehnice — și i se cere explicit să nu adauge nimic care nu este prezent în aceste date. Revizuiești fiecare FAQ sau descriere rescrisă înainte de publicare; nimic nu devine live automat.

**Ce se întâmplă cu datele mele dacă dezinstalez aplicația?**
Configurația magazinului tău, auditurile salvate, ciornele de FAQ și rescriere de conținut, prompt-urile de vizibilitate și evenimentele de trafic de recomandare AI sunt șterse automat când Shopify ne notifică despre dezinstalare. Aplicația nu păstrează nimic după ce pleci.

**Pot anula sau face downgrade fără să contactez asistența?**
Da. Mergi la **Prețuri** în aplicație și comută la Free oricând — intră în vigoare imediat, fără a fi nevoie de email.

## Limitele planurilor

| Funcționalitate | Free | Grow | Unlimited |
|---|---|---|---|
| Audit catalog | Primele 20 de produse, o singură dată, fără istoric | Catalog complet + istoric | Catalog complet + istoric |
| Simulator crawler | 20/lună | 300/lună | 1.000/lună |
| Comparație cu concurența | 10/lună | 50/lună | 150/lună |
| Generare FAQ | Neinclus | 500/lună | 500/lună |
| Rescriere conținut | Neinclus | 300/lună | 300/lună |
| Visibility AI (prompt-uri urmărite) | Neinclus | 5 prompt-uri | 15 prompt-uri |
| Pixel trafic de recomandare AI | Neinclus | Inclus | Inclus |
| Chat de asistență AI | 1.000 mesaje/lună | 1.000 mesaje/lună | 1.000 mesaje/lună |
| Limbi de interfață | Toate cele 30 | Toate cele 30 | Toate cele 30 |

Preț lunar: Free $0, Grow $9.99, Unlimited $19.99. Facturarea anuală pe Grow/Unlimited este aproximativ două luni gratuite comparativ cu plata lunară.

**De ce planul Free acoperă doar 20 de produse?**
Este menit să te lase să vezi rezultate reale pe propriul tău catalog înainte de a te angaja la un plan plătit. Grow și Unlimited elimină acest plafon și păstrează un istoric complet al auditurilor anterioare.

**Chiar există un plafon pentru generarea de FAQ, chiar și pe Unlimited?**
Da — 500 de generări pe lună, în mod deliberat, chiar și pe planul de top. Aceasta menține funcționalitatea sustenabilă la prețul actual; dacă ai un catalog de volum mare care are nevoie de mai mult, contactează-ne și găsim o soluție.

**De ce este chatul de asistență AI la fel pe fiecare plan?**
Este o decizie de produs, nu o omisiune: asistența este inclusă pentru toată lumea, niciodată un diferențiator plătit. Plafonul de mesaje (1.000/lună) există doar ca o măsură tehnică de protecție împotriva abuzului, nu ca o limită reală — nicio utilizare legitimă nu se apropie de el.

**Am găsit un bug sau ceva pare greșit. Cui îi spun?**
Scrie la [info@ifgecommerce.com](mailto:info@ifgecommerce.com) cu ce ai văzut și, dacă poți, ce produs sau pagină — de obicei este suficient pentru a-l identifica rapid. Poți folosi și chatul de asistență AI din aplicație și poți cere să vorbești cu un om.

[← Înapoi la Centrul de asistență](index.html)
