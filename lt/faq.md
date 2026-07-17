---
title: IFG GEO Optimizer
description: „IFG GEO Optimizer“ Shopify programos dokumentacija, DUK ir teisiniai puslapiai.
lang: lt
---

# Dažniausiai užduodami klausimai

<div class="lang-switcher">
{% include lang-switcher.html current="lt" slug="faq" %}
</div>

**Kuo skiriasi GEO nuo SEO?**
Tradicinė SEO optimizuoja paieškos varikliams, kurie reitinguoja ir išvardija nuorodas. GEO (Generative Engine Optimization) optimizuoja AI sistemoms, kurios skaito jūsų turinį ir tiesiogiai generuoja atsakymą ar rekomendaciją — ChatGPT, Perplexity, Gemini, Claude ir Google AI Overviews. Šios dvi sritys sutampa, tačiau GEO rūpi dalykai, kurių klasikiniai SEO įrankiai netikrina: ar jūsų produkto puslapyje yra pilni struktūrizuoti duomenys, ar AI crawler'is iš tikrųjų gali perskaityti jūsų turinį nevykdydamas JavaScript, ir ar jūsų tekstas parašytas taip, kad jį būtų lengva cituoti.

**Ar programa kada nors liečia mano klientų duomenis?**
Ne, jokių asmeninių klientų duomenų. Programos Shopify leidimai yra `read_products`, `write_products`, `read_themes` ir `write_pixels` — katalogo skaitymas ir tobulinimas, temos priedo aktyvavimo patikrinimas ir anoniminio parduotuvės srauto pikselio aktyvavimas (žr. žemiau). Ji niekada neprašo užsakymų ar klientų įrašų. Visą išsamią informaciją žr. [Privatumo politikoje](privacy.html).

**Kas yra AI nukreipiamo srauto pikselis, ir ar juo sekami mano klientai?**
Visuose planuose mažas Web Pixel aptinka, kada apsilankymas parduotuvės vitrinoje atkeliauja iš žinomo AI variklio (per naršyklės referrer) ir praneša variklį, puslapį bei laiko žymą — nieko, kas identifikuotų lankytoją, jokių slapukų, jokių sesijos duomenų. Jis veikia tik jei lankytojas jau davė sutikimą analitikai per jūsų parduotuvės slapukų juostą (Shopify Customer Privacy API). Naudojamas Dashboard plytelei rodyti ("AI nukreipiamas srautas, pastarosios 7 dienos") — tai AI matomumo stebėjimo atitikmuo, kuris parodo, ar esate minimi, bet ne tai, ar tas paminėjimas ką nors atsiuntė.

**Ką iš tikrųjų pakeičia mygtukas „Fix" katalogo audite?**
Jis įrašo trūkstamus schema.org struktūrizuotus duomenis į produkto metalauką (metafield) — pavyzdžiui, technines specifikacijas, išvestas iš jau esamų produkto parinkčių. Jis niekada neliečia produkto pavadinimo, aprašymo, nuotraukų ar kainos, ir niekada nesugalvoja duomenų, kurių negali patikrinti: pavyzdžiui, trūkstamas brūkšninis kodas taip ir lieka trūkstamas, o ne spėjamas.

**Ar DUK atsakymai ir perrašyti aprašymai yra AI sugalvoti, ar paremti mano realiu produktu?**
Modelis mato tik duomenis, kuriuos jau turite — pavadinimą, aprašymą, tiekėją ir technines specifikacijas — ir jam aiškiai nurodyta nieko nepridėti, ko tuose duomenyse nėra. Peržiūrite kiekvieną DUK ar perrašytą aprašymą prieš jam publikuojantis; niekas neatsiranda automatiškai.

**Kas nutinka mano duomenims, jei pašalinu programą?**
Jūsų parduotuvės konfigūracija, išsaugoti auditai, DUK ir turinio perrašymo juodraščiai, matomumo užklausos ir AI nukreipiamo srauto įvykiai automatiškai ištrinami, kai Shopify praneša mums apie pašalinimą. Programa nieko nepasilieka po to, kai išeinate.

**Ar galiu atsisakyti arba sumažinti planą nesikreipdamas į pagalbą?**
Taip. Eikite į **Pricing** programoje ir bet kada persijunkite į Free — tai įsigalioja iš karto, el. laiško rašyti nereikia.

## Plano limitai

| Funkcija | Free | Grow | Unlimited |
|---|---|---|---|
| Katalogo auditas | Pirmi 20 produktų, vienkartinis, be istorijos | Visas katalogas + istorija | Visas katalogas + istorija |
| Crawler simuliatorius | 20/mėn. | 300/mėn. | 1,000/mėn. |
| Konkurentų palyginimas | 10/mėn. | 50/mėn. | 150/mėn. |
| DUK generavimas | Neįtraukta | 500/mėn. | 500/mėn. |
| Turinio perrašymas | Neįtraukta | 300/mėn. | 300/mėn. |
| Visibility AI (sekamos užklausos) | Neįtraukta | 5 užklausos | 15 užklausų |
| AI nukreipiamo srauto pikselis | Įtraukta | Įtraukta | Įtraukta |
| AI pagalbos pokalbis | 1,000 žinučių/mėn. | 1,000 žinučių/mėn. | 1,000 žinučių/mėn. |
| Sąsajos kalbos | Visos 30 | Visos 30 | Visos 30 |

Mėnesio kaina: Free $0, Grow $9.99, Unlimited $19.99. Metinis apmokėjimas Grow/Unlimited planuose reiškia maždaug du mėnesius nemokamai, lyginant su mėnesiniu mokėjimu.

**Kodėl Free planas apima tik 20 produktų?**
Tai skirta leisti pamatyti realius rezultatus savo kataloge prieš įsipareigojant mokamam planui. Grow ir Unlimited panaikina šią ribą ir išsaugo pilną praeitų auditų istoriją.

**Ar tikrai yra riba DUK generavimui net Unlimited plane?**
Taip — 500 generavimų per mėnesį, sąmoningai, net aukščiausiame plane. Tai išlaiko funkciją tvarią prie dabartinės kainos; jei turite didelės apimties katalogą, kuriam reikia daugiau, susisiekite ir kartu ką nors sugalvosime.

**Kodėl AI pagalbos pokalbis vienodas visuose planuose?**
Tai produkto sprendimas, o ne apsirikimas: pagalba įtraukta visiems, niekada nėra mokamas diferenciatorius. Žinučių riba (1,000/mėn.) egzistuoja tik kaip techninė apsauga nuo piktnaudžiavimo, o ne kaip reali riba — joks teisėtas naudojimas prie jos net nepriartėja.

**Radau klaidą arba kažkas atrodo negerai. Kam pranešti?**
Rašykite [info@ifgecommerce.com](mailto:info@ifgecommerce.com), aprašydami, ką pastebėjote, ir, jei galite, nurodydami kurį produktą ar puslapį — dažniausiai to pakanka greitai tai išsiaiškinti. Taip pat galite naudotis AI pagalbos pokalbiu programos viduje ir paprašyti pakalbėti su žmogumi.

[← Atgal į Pagalbos centrą](index.html)
