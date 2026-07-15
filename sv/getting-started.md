---
title: IFG GEO Optimizer
description: Dokumentation, FAQ och juridiska sidor för Shopify-appen IFG GEO Optimizer.
lang: sv
---

# Komma igång

<div class="lang-switcher">
{% include lang-switcher.html current="sv" slug="getting-started" %}
</div>

IFG GEO Optimizer har nio områden, alla nåbara från den övre navigeringen när installationen är klar: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** och **Support**. Den här guiden går igenom alla, i den ordning de flesta handlare använder dem.

## 1. Installera och slutför installationsguiden

Vid första öppningen samlar en kort guidad installation (cirka 2 minuter) in grunderna: gränssnittsspråk, dina retur- och fraktpolicyuppgifter, din företagsinformation och — det enda steget som faktiskt spelar teknisk roll — aktivering av app-inbäddningen **GEO Schema** i din temaredigerare. Inget av det appen gör efteråt når din butiksfront förrän den här inbäddningen är aktiverad, så det är värt att inte hoppa över den. Du kan alltid ändra något av dessa svar senare från **Settings**.

## 2. Dashboard

Din startbas. Den visar din aktuella GEO-poäng (från din senaste audit), en **Readiness Matrix** med åtta signaler på ett ögonkast — innehållsextraherbarhet, Organization-schema, `llms.txt`, `agents.md`, crawler-åtkomst, MCP-beredskap, Link Coach-anslutning och AI-hänvisningstrafik — plus en prioriterad "fixa detta först"-lista och din plans användningsräknare (FAQ-genereringar, katalogstorlek). Allt här länkar direkt till sidan där du kan agera på det.

## 3. Audit catalog

Klicka på **Rescan catalog** för att kontrollera varje produkt mot nio fält med strukturerad data som sökmotorer letar efter: bild, beskrivning, varumärke, SKU, GTIN, pris, tekniska specifikationer, returpolicy och fraktpolicy. Produkter under 80/100 visar exakt vad som saknas.

- **Ett-klicks-fix**: där appen på ett säkert sätt kan härleda den saknade datan (oftast tekniska specifikationer från dina befintliga produktalternativ) ser du en **Fix**-knapp som skriver den direkt till produktens strukturerade data. Inget gissas för fält som appen inte kan verifiera — en saknad streckkod, till exempel, förblir saknad istället för att uppfinnas.
- **Content chunking-poäng**: vid sidan av kontrollen av strukturerad data får varje produkt en separat extraherbarhetspoäng — inte "finns fältet" utan "kan ett AI/RAG-system faktiskt hämta ett rent faktum ur den här beskrivningen." Tunn text med mycket adjektiv får lägre poäng även med perfekt schema.org-markup.
- **`llms.txt`**: genererar en riktig, standardkompatibel `llms.txt`-fil som sammanfattar din katalog för AI-system, levererad på din butiks verkliga rot (`/llms.txt`), inte begravd under en app-proxy-sökväg där crawlers inte hittar den.
- **`agents.md`**: genererar en fil som beskriver din butik för autonoma shoppingagenter — varianter, sökning, kassa — byggd endast av verklig data som din butik redan exponerar, inget uppfunnet.
- **Organization-schema**: publicerar din företagsinformation (juridiskt namn, moms-/skatte-ID, adress) som strukturerad data, så att AI-motorer kan verifiera att du är ett riktigt, ansvarigt företag innan de rekommenderar dig.

På Free täcker audits dina första 20 produkter, en gång, utan sparad historik. Grow och Unlimited skannar hela din katalog och sparar varje tidigare skanning för trendjämförelse.

## 4. Crawler AI

Välj en produkt så hämtar appen dess sida exakt så som en AI-crawler gör — utan JavaScript-körning, precis som GPTBot, ClaudeBot eller PerplexityBot — så att du ser exakt vad som är synligt för dessa motorer: om din `robots.txt` blockerar dem (kontrollerat per bot, inte bara ett generiskt tillåt/neka), och om din strukturerade data faktiskt överlever i den rå HTML som dessa botar läser.

**Konkurrentjämförelse** (egen flik på den här sidan): klistra in en konkurrents produkt-URL och få samma GEO-signaler jämförda sida vid sida med dina — samma typ av skillnad du skulle få av en manuell audit, utan att behöva registrera dig för konkurrentens egna verktyg.

## 5. FAQ product

På Grow eller Unlimited väljer du en produkt och klickar på **Generate FAQs** för tre till fem frågor-och-svar-par som utformas enbart utifrån produktens verkliga titel, beskrivning, leverantör och specifikationer — modellen är uttryckligen instruerad att aldrig lägga till en detalj som inte redan finns i din data. Granska varje utkast; inget publiceras utan ditt uttryckliga **Approve**. Godkända FAQ visas på den publicerade produktsidan och märks upp som `FAQPage`-strukturerad data, så de är både läsbara för människor och citerbara för maskiner.

**Omskrivning av innehåll** (egen flik på den här sidan): appen kan skriva om en produktbeskrivning så att den blir tätare med verifierbara fakta och lättare för en generativ motor att citera — du ser alltid en jämförelse före/efter och godkänner innan något skrivs tillbaka till produkten.

## 6. Link Coach

Analyserar hur väl dina produkter är sammankopplade genom delade kollektioner, leverantörer och taggar — intern länkning är en signal som AI-system använder för att förstå vad din katalog täcker som helhet, inte bara en sida i taget. Visar övergivna produkter utan meningsfulla kopplingar och förklarbara förslag för att åtgärda det.

## 7. Visibility AI

Lägg till upp till ett handfull prompter du realistiskt kan förvänta dig att en kund skulle fråga en AI-assistent (gränsen beror på din plan — se Pricing nedan), och varje vecka kontrollerar appen om Claude, ChatGPT, Gemini och Perplexity nämner din butik i svaret, spårat över tid per motor. På Grow och Unlimited visar detta även hur du jämför dig med namngivna konkurrenter på samma prompter.

**AI-hänvisningstrafik** (Grow och Unlimited): en lättviktig, integritetsrespekterande pixel upptäcker när ett besök i butiksfronten faktiskt kommer från en av dessa AI-motorer (via referrer, endast efter att besökaren gett analyssamtycke via din butiks cookiebanner) och rapporterar hur många sådana besök du fick de senaste 7 dagarna — den andra halvan av loopen som enbart visibility-spårning inte kan visa: inte bara "nämns vi," utan "skickar den nämningen någon till oss."

## 8. Support

En AI-chattassistent finns i appen (ikon nere till höger) för frågor om GEO, dina auditresultat eller hur en specifik funktion fungerar. Om den inte kan hjälpa kan du be om att få prata med en människa, och konversationen vidarebefordras direkt till IFG eCommerce.

## 9. Settings

Här hanterar du svaren från installationsguiden (policyer, företagsdata, gränssnittsspråk — byt omedelbart mellan 30 språk, utan laddningsfördröjning), kontrollerar temainbäddningens aktivering på nytt och ser ditt kontos Shopify-behörigheter (scopes).

## 10. Pricing

**Pricing** visar Free, Grow och Unlimited sida vid sida, månadsvis eller årsvis (årsvis motsvarar ungefär 2 gratis månader på båda betalplanerna). Du kan uppgradera, nedgradera eller avbryta tillbaka till Free när som helst, direkt från appen — inget e-postmeddelande krävs. Se [FAQ](faq.html) för exakta plangränser.

Det är hela loopen. De flesta handlare kör om en audit efter att ha lagt till nya produkter, kontrollerar crawler-simulatorn varje gång de uppdaterar en beskrivning, och kastar en blick på Dashboardens Readiness Matrix varje vecka.

[← Tillbaka till Hjälpcenter](index.html)
