---
title: IFG GEO Optimizer
description: Dokumentation, FAQ och juridiska sidor för Shopify-appen IFG GEO Optimizer.
lang: sv
---

# Vanliga frågor

<div class="lang-switcher">
{% include lang-switcher.html current="sv" slug="faq" %}
</div>

**Vad är skillnaden mellan GEO och SEO?**
Traditionell SEO optimerar för sökmotorer som rankar och listar länkar. GEO (Generative Engine Optimization) optimerar för AI-system som läser ditt innehåll och genererar ett svar eller en rekommendation direkt — ChatGPT, Perplexity, Gemini, Claude och Google AI Overviews. De två överlappar, men GEO bryr sig om saker klassiska SEO-verktyg inte kontrollerar: om din produktsida har komplett strukturerad data, om en AI-crawler faktiskt kan läsa ditt innehåll utan att köra JavaScript, och om din text är skriven på ett sätt som är lätt att citera.

**Rör appen någonsin mina kunders data?**
Nej, ingen personlig kunddata. Appens Shopify-behörigheter är `read_products`, `write_products`, `read_themes` och `write_pixels` — att läsa och förbättra din katalog, kontrollera att temainbäddningen är aktiv, och aktivera en anonym pixel för butiksfrontstrafik (se nedan). Den begär aldrig ordrar eller kunduppgifter. Se [Integritetspolicyn](privacy.html) för hela genomgången.

**Vad är AI-hänvisningstrafikpixeln, och spårar den mina kunder?**
På Grow och Unlimited upptäcker en liten Web Pixel när ett besök i butiksfronten kommer från en känd AI-motor (via webbläsarens referrer) och rapporterar motorn, sidan och en tidsstämpel — inget som identifierar besökaren, inga cookies, ingen sessionsdata. Den körs bara om besökaren redan gett analyssamtycke via din butiks cookiebanner (Shopifys Customer Privacy API). Den används för att visa en Dashboard-ruta ("AI-hänvisningstrafik, senaste 7 dagarna") — motsvarigheten till Visibility AI-spårningen, som talar om ifall du nämns men inte om den nämningen skickade någon till dig.

**Vad ändrar egentligen "Fix"-knappen i katalogauditen?**
Den skriver saknad schema.org-strukturerad data till ett produktmetafält — saker som tekniska specifikationer härledda från dina befintliga produktalternativ. Den rör aldrig din produkttitel, beskrivning, bilder eller pris, och den hittar aldrig på data den inte kan verifiera: en saknad streckkod, till exempel, förblir saknad istället för att gissas fram.

**Är FAQ-svaren och omskrivna beskrivningarna påhittade av AI, eller baserade på min faktiska produkt?**
Modellen ser bara den produktdata du redan har — titel, beskrivning, leverantör och tekniska specifikationer — och är uttryckligen instruerad att inte lägga till något som inte finns i den datan. Du granskar varje FAQ eller omskriven beskrivning innan den publiceras; inget går live automatiskt.

**Vad händer med min data om jag avinstallerar appen?**
Din butikskonfiguration, sparade audits, FAQ- och innehållsomskrivningsutkast, visibility-prompter och AI-hänvisningstrafikhändelser raderas automatiskt när Shopify meddelar oss om avinstallationen. Appen behåller inget efter att du lämnat.

**Kan jag avbryta eller nedgradera utan att kontakta supporten?**
Ja. Gå till **Pricing** i appen och byt till Free när som helst — det träder i kraft omedelbart, inget e-postmeddelande krävs.

## Plangränser

| Funktion | Free | Grow | Unlimited |
|---|---|---|---|
| Katalogaudit | Första 20 produkterna, en gång, ingen historik | Hela katalogen + historik | Hela katalogen + historik |
| Crawler-simulator | 20/månad | 300/månad | 1 000/månad |
| Konkurrentjämförelse | 10/månad | 50/månad | 150/månad |
| FAQ-generering | Ingår ej | 500/månad | 500/månad |
| Omskrivning av innehåll | Ingår ej | 300/månad | 300/månad |
| Visibility AI (spårade prompter) | Ingår ej | 5 prompter | 15 prompter |
| AI-hänvisningstrafikpixel | Ingår ej | Ingår | Ingår |
| AI-supportchatt | 1 000 meddelanden/månad | 1 000 meddelanden/månad | 1 000 meddelanden/månad |
| Gränssnittsspråk | Alla 30 | Alla 30 | Alla 30 |

Månadspriser: Free $0, Grow $9.99, Unlimited $19.99. Årsvis fakturering på Grow/Unlimited motsvarar ungefär två gratis månader jämfört med månadsvis betalning.

**Varför täcker Free-planen bara 20 produkter?**
Det är tänkt att låta dig se verkliga resultat på din egen katalog innan du bestämmer dig för en betalplan. Grow och Unlimited tar bort den gränsen och sparar en fullständig historik över tidigare audits.

**Finns det verkligen ett tak för FAQ-generering även på Unlimited?**
Ja — 500 genereringar i månaden, medvetet, även på den högsta planen. Det håller funktionen hållbar till nuvarande pris; om du har en högvolymkatalog som behöver mer, hör av dig så löser vi något.

**Varför är AI-supportchatten samma på alla planer?**
Det är ett produktbeslut, inte ett förbiseende: support ingår för alla, aldrig en betald differentierare. Meddelandetaket (1 000/månad) finns bara som ett tekniskt skydd mot missbruk, inte som en praktisk begränsning — ingen legitim användning kommer i närheten av det.

**Jag hittade en bugg eller något som ser fel ut. Vem berättar jag för?**
Skicka e-post till [info@ifgecommerce.com](mailto:info@ifgecommerce.com) med vad du såg och, om möjligt, vilken produkt eller sida — det räcker vanligtvis för att snabbt spåra det. Du kan även använda AI-supportchatten i appen och be om att få prata med en människa.

[← Tillbaka till Hjälpcenter](index.html)
