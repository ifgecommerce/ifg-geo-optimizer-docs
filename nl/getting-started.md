---
title: IFG GEO Optimizer
description: Documentatie, veelgestelde vragen en juridische pagina's voor de Shopify-app IFG GEO Optimizer.
lang: nl
---

# Aan de slag

<div class="lang-switcher">
{% include lang-switcher.html current="nl" slug="getting-started" %}
</div>

IFG GEO Optimizer heeft negen onderdelen, allemaal bereikbaar via de bovenste navigatie zodra de installatie is voltooid: **Dashboard**, **Catalogusaudit**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Prijzen**, **Instellingen** en **Ondersteuning**. Deze gids doorloopt ze allemaal, in de volgorde waarin de meeste winkeliers ze gebruiken.

## 1. Installeer en doorloop de installatiewizard

Bij de eerste keer openen verzamelt een korte begeleide installatie (ongeveer 2 minuten) de basisgegevens: interfacetaal, de details van je retour- en verzendbeleid, je bedrijfsgegevens en — de enige stap die technisch echt van belang is — het activeren van de **GEO Schema** app-embed in de themabewerker. Niets van wat de app daarna doet, bereikt je storefront totdat deze embed is ingeschakeld, dus het loont om deze stap niet over te slaan. Je kunt al deze antwoorden later altijd wijzigen via **Instellingen**.

## 2. Dashboard

Je uitvalsbasis. Hier zie je je huidige GEO-score (van je laatste audit), een **Readiness Matrix** met acht signalen in één oogopslag — content-extraheerbaarheid, Organization schema, `llms.txt`, `agents.md`, crawlertoegang, MCP-gereedheid, Link Coach-connectiviteit en AI-doorverwijzingsverkeer — plus een geprioriteerde lijst met "los dit eerst op" en de gebruikstellers van je pakket (FAQ-generaties, catalogusomvang). Alles hier linkt rechtstreeks naar de pagina waar je actie kunt ondernemen.

## 3. Catalogusaudit

Klik op **Catalogus opnieuw scannen** om elk product te controleren tegen negen gestructureerde-datavelden waar zoekmachines naar kijken: afbeelding, beschrijving, merk, SKU, GTIN, prijs, technische specificaties, retourbeleid en verzendbeleid. Producten onder 80/100 laten precies zien wat er ontbreekt.

- **One-click fix**: waar de app de ontbrekende data veilig kan afleiden (meestal technische specificaties uit je bestaande productopties), zie je een knop **Herstellen** die de data direct naar de gestructureerde data van het product schrijft. Er wordt niets geraden voor velden die de app niet kan verifiëren — een ontbrekende barcode blijft bijvoorbeeld ontbrekend in plaats van verzonnen te worden.
- **Content chunking score**: naast de controle op gestructureerde data krijgt elk product een aparte extraheerbaarheidsscore — niet "is het veld aanwezig" maar "kan een AI/RAG-systeem hier echt een schoon feit uit halen." Dunne, bijvoeglijk-naamwoord-zware teksten scoren lager, zelfs met perfecte schema.org-markup.
- **`llms.txt`**: genereert een echt, standaardconform `llms.txt`-bestand dat je catalogus samenvat voor AI-systemen, geserveerd op de echte root van je winkel (`/llms.txt`), niet verstopt onder een app-proxypad waar crawlers het niet vinden.
- **`agents.md`**: genereert een bestand dat je winkel beschrijft aan autonome shopping agents — varianten, zoeken, checkout — uitsluitend opgebouwd uit echte data die je winkel al blootstelt, niets verzonnen.
- **Organization schema**: publiceert je bedrijfsgegevens (statutaire naam, btw-/belastingnummer, adres) als gestructureerde data, zodat AI-engines kunnen verifiëren dat je een echt, aansprakelijk bedrijf bent voordat ze je aanbevelen.

Op Free dekt de audit je eerste 20 producten, eenmalig, zonder geschiedenis. Grow en Unlimited scannen je hele catalogus en bewaren elke eerdere scan voor trendvergelijking.

## 4. Crawler AI

Kies een product en de app haalt de pagina exact op zoals een AI-crawler dat doet — zonder JavaScript-uitvoering, net als GPTBot, ClaudeBot of PerplexityBot — zodat je precies ziet wat zichtbaar is voor deze engines: of je `robots.txt` ze blokkeert (per bot gecontroleerd, niet alleen een generieke toestaan/blokkeren), en of je gestructureerde data daadwerkelijk overeind blijft in de ruwe HTML die deze bots lezen.

**Concurrentievergelijking** (eigen tabblad op deze pagina): plak de productURL van een concurrent en krijg dezelfde GEO-signalen naast elkaar vergeleken met die van jou — hetzelfde soort verschil dat je van een handmatige audit zou krijgen, zonder je te hoeven aanmelden bij de eigen tools van de concurrent.

## 5. FAQ product

Op Grow of Unlimited kies je een product en klik je op **FAQ's genereren** voor drie tot vijf vraag-antwoordparen die uitsluitend zijn opgesteld op basis van de echte titel, beschrijving, leverancier en specificaties van dat product — het model krijgt de uitdrukkelijke instructie om nooit een detail toe te voegen dat nog niet in je data staat. Beoordeel elk concept; niets wordt gepubliceerd zonder je expliciete **Goedkeuren**. Goedgekeurde FAQ's verschijnen op de live productpagina en worden gemarkeerd als `FAQPage`-gestructureerde data, zodat ze zowel door mensen leesbaar als door machines citeerbaar zijn.

**Content herschrijven** (eigen tabblad op deze pagina): de app kan een productbeschrijving herschrijven zodat deze dichter met verifieerbare feiten is gevuld en makkelijker te citeren is voor een generative engine — je ziet altijd een vergelijking voor/na en keurt goed voordat er iets teruggeschreven wordt naar het product.

## 6. Link Coach

Analyseert hoe goed je producten met elkaar verbonden zijn via gedeelde collecties, leveranciers en tags — interne links zijn een signaal dat AI-systemen gebruiken om te begrijpen wat je catalogus als geheel omvat, niet slechts één pagina tegelijk. Toont geïsoleerde producten zonder zinvolle verbindingen en uitlegbare suggesties om dat op te lossen.

## 7. Visibility AI

Voeg tot een handvol prompts toe die je realistisch zou verwachten dat een klant aan een AI-assistent stelt (de limiet hangt af van je pakket — zie Prijzen hieronder), en elke week controleert de app of Claude, ChatGPT, Gemini en Perplexity je winkel noemen in het antwoord, per engine bijgehouden in de tijd. Op Grow en Unlimited zie je ook hoe je scoort ten opzichte van met naam genoemde concurrenten op dezelfde prompts.

**AI-doorverwijzingsverkeer** (Grow en Unlimited): een lichte, privacyvriendelijke pixel detecteert wanneer een bezoek aan de storefront daadwerkelijk afkomstig is van een van deze AI-engines (via de referrer, alleen nadat de bezoeker toestemming heeft gegeven voor analytics via de cookiebanner van je winkel) en rapporteert hoeveel van dit soort bezoeken je de afgelopen 7 dagen had — de andere helft van het plaatje die visibility tracking alleen niet kan laten zien: niet alleen "worden we genoemd," maar "stuurt die vermelding ook iemand door."

## 8. Ondersteuning

Een AI-chatassistent leeft in de app (icoon rechtsonder) voor vragen over GEO, je auditresultaten, of hoe een specifieke functie werkt. Als die niet kan helpen, kun je vragen om met een mens te spreken en wordt het gesprek rechtstreeks doorgestuurd naar IFG eCommerce.

## 9. Instellingen

Hier beheer je de antwoorden van de installatiewizard (beleid, bedrijfsgegevens, interfacetaal — direct wisselen tussen 30 talen, zonder vertraging), controleer je opnieuw of de thema-embed actief is, en zie je de Shopify-scopes van je account.

## 10. Prijzen

**Prijzen** toont Free, Grow en Unlimited naast elkaar, maandelijks of jaarlijks (jaarlijks is ruwweg 2 maanden gratis op beide betaalde pakketten). Je kunt op elk moment upgraden, downgraden, of terug naar Free annuleren, rechtstreeks vanuit de app — geen e-mail nodig. Zie de [Veelgestelde vragen](faq.html) voor de exacte pakketlimieten.

Dat is de volledige cyclus. De meeste winkeliers voeren opnieuw een audit uit na het toevoegen van nieuwe producten, controleren de crawler simulator telkens wanneer ze een beschrijving bijwerken, en werpen wekelijks een blik op de Readiness Matrix van het Dashboard.

[← Terug naar Helpcentrum](index.html)
