---
title: IFG GEO Optimizer
description: Dokumentacija, česta pitanja i pravne stranice za Shopify aplikaciju IFG GEO Optimizer.
lang: hr
---

# Česta pitanja

<div class="lang-switcher">
{% include lang-switcher.html current="hr" slug="faq" %}
</div>

**Koja je razlika između GEO-a i SEO-a?**
Tradicionalni SEO optimizira za tražilice koje rangiraju i prikazuju popise poveznica. GEO (Generative Engine Optimization) optimizira za AI sustave koji čitaju vaš sadržaj i izravno generiraju odgovor ili preporuku — ChatGPT, Perplexity, Gemini, Claude i Google AI Overviews. Ova dva pristupa se preklapaju, ali GEO-u je stalo do stvari koje klasični SEO alati ne provjeravaju: ima li vaša stranica proizvoda potpune strukturirane podatke, može li AI crawler zaista pročitati vaš sadržaj bez izvršavanja JavaScripta, te je li vaš tekst napisan na način koji je lako citirati.

**Dodiruje li aplikacija ikada podatke mojih kupaca?**
Ne, nikakve osobne podatke kupaca. Shopify dozvole aplikacije su `read_products`, `write_products`, `read_themes` i `write_pixels` — čitanje i poboljšavanje vašeg kataloga, provjera je li embed teme aktivan i aktivacija anonimnog piksela prometa trgovine (vidi niže). Nikada ne zahtijeva narudžbe ni evidencije kupaca. Pogledajte [Pravila privatnosti](privacy.html) za potpuni pregled.

**Što je piksel AI referral prometa i prati li moje kupce?**
Na svakom planu, mali Web Pixel otkriva kada posjet trgovini stiže od poznatog AI motora (putem referrera preglednika) i izvještava o motoru, stranici i vremenskoj oznaci — ništa što identificira posjetitelja, bez kolačića, bez podataka o sesiji. Pokreće se samo ako je posjetitelj već dao pristanak za analitiku putem bannera kolačića vaše trgovine (Shopify Customer Privacy API). Koristi se za prikaz pločice na Dashboardu ("AI referral promet, posljednjih 7 dana") — protuteža praćenju Visibility AI, koje vam govori jeste li spomenuti, ali ne i je li to spominjanje nekoga poslalo.

**Što točno mijenja gumb "Ispravi" u auditu kataloga?**
Upisuje nedostajuće schema.org strukturirane podatke u metapolje (metafield) proizvoda — stvari poput tehničkih specifikacija izvedenih iz postojećih opcija proizvoda. Nikada ne dira naziv, opis, slike ili cijenu vašeg proizvoda, i nikada ne izmišlja podatke koje ne može provjeriti: nedostajući barkod, primjerice, ostaje nedostajući umjesto da se pogađa.

**Jesu li FAQ odgovori i prepisani opisi izmišljeni od strane AI-a, ili se temelje na mom stvarnom proizvodu?**
Model vidi samo podatke o proizvodu koje već imate — naziv, opis, dobavljača i tehničke specifikacije — i izričito je upućen da ne dodaje ništa što nije prisutno u tim podacima. Pregledavate svaki FAQ ili prepisani opis prije objave; ništa ne ide uživo automatski.

**Što se događa s mojim podacima ako deinstaliram aplikaciju?**
Konfiguracija vaše trgovine, spremljeni auditi, nacrti FAQ-a i prepisanog sadržaja, upiti za vidljivost i događaji AI referral prometa automatski se brišu kada Shopify obavijesti o deinstalaciji. Aplikacija ne zadržava ništa nakon što odete.

**Mogu li otkazati ili downgradati bez kontaktiranja podrške?**
Da. Idite na **Cjenik** unutar aplikacije i prebacite se na Free u bilo kojem trenutku — stupa na snagu odmah, bez potrebe za e-mailom.

## Ograničenja po planu

| Značajka | Free | Grow | Unlimited |
|---|---|---|---|
| Audit kataloga | Prvih 20 proizvoda, jednokratno, bez povijesti | Cijeli katalog + povijest | Cijeli katalog + povijest |
| Simulator crawlera | 20/mjesec | 300/mjesec | 1.000/mjesec |
| Usporedba s konkurencijom | 10/mjesec | 50/mjesec | 150/mjesec |
| Generiranje FAQ-a | Nije uključeno | 500/mjesec | 500/mjesec |
| Prepisivanje sadržaja | Nije uključeno | 300/mjesec | 300/mjesec |
| Visibility AI (praćeni upiti) | Nije uključeno | 5 upita | 15 upita |
| Piksel AI referral prometa | Uključeno | Uključeno | Uključeno |
| AI chat podrška | 1.000 poruka/mjesec | 1.000 poruka/mjesec | 1.000 poruka/mjesec |
| Jezici sučelja | Svih 30 | Svih 30 | Svih 30 |

Mjesečne cijene: Free $0, Grow $9.99, Unlimited $19.99. Godišnja naplata na Grow/Unlimited otprilike je dva mjeseca besplatno u usporedbi s mjesečnim plaćanjem.

**Zašto Free plan obuhvaća samo 20 proizvoda?**
Cilj je da vidite stvarne rezultate na vlastitom katalogu prije nego što se obvežete na plaćeni plan. Grow i Unlimited uklanjaju taj limit i čuvaju potpunu povijest prošlih audita.

**Postoji li stvarno ograničenje generiranja FAQ-a čak i na Unlimited planu?**
Da — 500 generiranja mjesečno, namjerno, čak i na najvišem planu. Ovo održava značajku održivom uz trenutnu cijenu; ako imate katalog velikog obujma kojem treba više, javite nam se i pronaći ćemo rješenje.

**Zašto je AI chat podrška ista na svakom planu?**
To je proizvodna odluka, ne propust: pomoć je uključena za sve, nikad plaćeni diferencijator. Ograničenje broja poruka (1.000/mjesec) postoji samo kao tehnička zaštita od zlouporabe, ne kao stvarno ograničenje — nijedna legitimna upotreba se tome ni približava.

**Pronašao/pronašla sam grešku ili nešto ne izgleda kako treba. Kome da javim?**
Pošaljite e-mail na [info@ifgecommerce.com](mailto:info@ifgecommerce.com) s onim što ste vidjeli i, ako možete, kojem proizvodu ili stranici — obično je to dovoljno za brzo pronalaženje uzroka. Možete koristiti i AI chat podršku unutar aplikacije i zatražiti razgovor s čovjekom.

[← Natrag na Centar za pomoć](index.html)
