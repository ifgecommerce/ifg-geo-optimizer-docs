---
title: IFG GEO Optimizer
description: Documentatie, veelgestelde vragen en juridische pagina's voor de Shopify-app IFG GEO Optimizer.
lang: nl
---

# Veelgestelde vragen

<div class="lang-switcher">
{% include lang-switcher.html current="nl" slug="faq" %}
</div>

**Wat is het verschil tussen GEO en SEO?**
Traditionele SEO optimaliseert voor zoekmachines die links rangschikken en weergeven. GEO (Generative Engine Optimization) optimaliseert voor AI-systemen die je content lezen en rechtstreeks een antwoord of aanbeveling genereren — ChatGPT, Perplexity, Gemini, Claude en Google AI Overviews. De twee overlappen, maar GEO houdt rekening met dingen die klassieke SEO-tools niet controleren: of je productpagina volledige gestructureerde data heeft, of een AI-crawler je content daadwerkelijk kan lezen zonder JavaScript uit te voeren, en of je tekst zo geschreven is dat hij makkelijk te citeren en aan te halen is.

**Komt de app ooit in aanraking met de gegevens van mijn klanten?**
Geen persoonlijke klantgegevens. De Shopify-permissies van de app zijn `read_products`, `write_products`, `read_themes` en `write_pixels` — voor het lezen en verbeteren van je catalogus, het controleren of de thema-embed actief is, en het activeren van een anonieme storefront-verkeerspixel (zie hieronder). De app vraagt nooit toegang tot bestellingen of klantgegevens. Zie het [Privacybeleid](privacy.html) voor het volledige overzicht.

**Wat is de pixel voor AI-doorverwijzingsverkeer, en volgt die mijn klanten?**
Op elk pakket detecteert een kleine Web Pixel wanneer een bezoek aan de storefront afkomstig is van een bekende AI-engine (via de browser-referrer) en registreert de engine, de pagina en een tijdstempel — niets wat de bezoeker identificeert, geen cookies, geen sessiedata. De pixel draait alleen als de bezoeker al toestemming heeft gegeven voor analytics via de cookiebanner van je winkel (de Customer Privacy API van Shopify). Dit voedt een tegel op het Dashboard ("AI-doorverwijzingsverkeer, laatste 7 dagen") — het complement van de Visibility AI-tracking, die laat zien of je genoemd wordt maar niet of die vermelding ook iemand doorstuurt.

**Wat verandert de knop "Herstellen" bij de catalogusaudit precies?**
Deze schrijft ontbrekende schema.org-gestructureerde data naar een productmetafield — zoals technische specificaties afgeleid van je bestaande productopties. De knop raakt nooit je producttitel, beschrijving, afbeeldingen of prijs aan, en verzint nooit data die niet te verifiëren is: een ontbrekende barcode blijft bijvoorbeeld ontbrekend in plaats van geraden te worden.

**Zijn de FAQ-antwoorden en herschreven beschrijvingen door AI verzonnen, of gebaseerd op mijn echte product?**
Het model ziet alleen de productdata die je al hebt — titel, beschrijving, leverancier en technische specificaties — en krijgt de uitdrukkelijke instructie niets toe te voegen dat niet in die data aanwezig is. Je beoordeelt elke FAQ of herschreven beschrijving voordat deze wordt gepubliceerd; niets gaat automatisch live.

**Wat gebeurt er met mijn gegevens als ik de app verwijder?**
Je winkelconfiguratie, opgeslagen audits, FAQ- en content-herschrijfconcepten, visibility-prompts en AI-doorverwijzingsverkeergebeurtenissen worden automatisch verwijderd zodra Shopify ons op de hoogte stelt van de deïnstallatie. De app houdt niets vast nadat je bent vertrokken.

**Kan ik opzeggen of downgraden zonder contact op te nemen met support?**
Ja. Ga naar **Prijzen** in de app en schakel op elk moment over naar Free — dit gaat direct in, geen e-mail nodig.

## Pakketlimieten

| Functie | Free | Grow | Unlimited |
|---|---|---|---|
| Catalogusaudit | Eerste 20 producten, eenmalig, geen geschiedenis | Volledige catalogus + geschiedenis | Volledige catalogus + geschiedenis |
| Crawler simulator | 20/maand | 300/maand | 1.000/maand |
| Concurrentievergelijking | 10/maand | 50/maand | 150/maand |
| FAQ-generatie | Niet inbegrepen | 500/maand | 500/maand |
| Content herschrijven | Niet inbegrepen | 300/maand | 300/maand |
| Visibility AI (gevolgde prompts) | Niet inbegrepen | 5 prompts | 15 prompts |
| Pixel voor AI-doorverwijzingsverkeer | Inbegrepen | Inbegrepen | Inbegrepen |
| AI-supportchat | 1.000 berichten/maand | 1.000 berichten/maand | 1.000 berichten/maand |
| Interfacetalen | Alle 30 | Alle 30 | Alle 30 |

Maandelijkse prijzen: Free $0, Grow $9,99, Unlimited $19,99. Jaarlijkse facturering op Grow/Unlimited komt neer op ongeveer twee maanden gratis vergeleken met maandelijks betalen.

**Waarom dekt het Free-pakket maar 20 producten?**
Dat is bedoeld om je echte resultaten op je eigen catalogus te laten zien voordat je je vastlegt op een betaald pakket. Grow en Unlimited verwijderen dat plafond en bewaren een volledige geschiedenis van eerdere audits.

**Is er echt een limiet op FAQ-generatie, zelfs op Unlimited?**
Ja — 500 generaties per maand, bewust, zelfs op het topplan. Dit houdt de functie betaalbaar bij de huidige prijs; als je een catalogus met hoog volume hebt en meer nodig hebt, neem dan contact op en we zoeken samen een oplossing.

**Waarom is de AI-supportchat op elk pakket hetzelfde?**
Dat is een productbeslissing, geen omissie: ondersteuning is voor iedereen inbegrepen, nooit een betaald onderscheid. Het berichtenplafond (1.000/maand) bestaat alleen als technische bescherming tegen misbruik, niet als een reëel limiet — geen enkel legitiem gebruik komt hier ook maar in de buurt van.

**Ik heb een bug gevonden of iets klopt niet. Aan wie meld ik dat?**
Mail naar [info@ifgecommerce.com](mailto:info@ifgecommerce.com) met wat je zag en, indien mogelijk, welk product of welke pagina het betrof — dat is meestal genoeg om het snel op te sporen. Je kunt ook de AI-supportchat in de app gebruiken en vragen om met een mens te spreken.

[← Terug naar Helpcentrum](index.html)
