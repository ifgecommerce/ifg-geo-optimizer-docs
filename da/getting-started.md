---
title: IFG GEO Optimizer
description: Dokumentation, FAQ og juridiske sider til Shopify-appen IFG GEO Optimizer.
lang: da
---

# Kom godt i gang

<div class="lang-switcher">
{% include lang-switcher.html current="da" slug="getting-started" %}
</div>

IFG GEO Optimizer har ni områder, som alle kan tilgås fra topnavigationen, når opsætningen er gennemført: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** og **Support**. Denne guide gennemgår dem alle, i den rækkefølge de fleste forhandlere bruger dem.

## 1. Installer og gennemfør opsætningsguiden

Ved første åbning samler en kort guidet opsætning (ca. 2 minutter) det grundlæggende: grænsefladesprog, detaljer om din returnerings- og forsendelsespolitik, dine virksomhedsoplysninger — og det ene trin, der faktisk har teknisk betydning — aktivering af app-embedden **GEO Schema** i din temaeditor. Intet, appen foretager sig bagefter, når din storefront, før denne embed er slået til, så det er værd ikke at springe over. Du kan altid ændre nogen af disse svar senere fra **Settings**.

## 2. Dashboard

Din base. Den viser din aktuelle GEO-score (fra din seneste audit), en **Readiness Matrix** med otte signaler på et øjeblik — indholdsudtrækkelighed, Organization-schema, `llms.txt`, `agents.md`, crawler-adgang, MCP-parathed, Link Coach-konnektivitet og AI-henvisningstrafik — plus en prioriteret "ret dette først"-liste og din plans forbrugstællere (FAQ-genereringer, katalogstørrelse). Alt her linker direkte til den side, hvor du kan handle på det.

## 3. Audit catalog

Klik på **Rescan catalog** for at tjekke hvert produkt mod ni strukturerede-data-felter, som søgemaskiner leder efter: billede, beskrivelse, mærke, SKU, GTIN, pris, tekniske specifikationer, returpolitik og forsendelsespolitik. Produkter under 80/100 viser præcis, hvad der mangler.

- **Et-klik-rettelse**: hvor appen sikkert kan udlede de manglende data (som regel tekniske specifikationer ud fra dine eksisterende produktvalgmuligheder), ser du en **Fix**-knap, der skriver dem direkte til produktets strukturerede data. Intet gættes for felter, appen ikke kan verificere — en manglende stregkode forbliver f.eks. manglende i stedet for at blive opfundet.
- **Content chunking-score**: ud over kontrollen af strukturerede data får hvert produkt en separat udtrækkelighedsscore — ikke "er feltet til stede", men "kan et AI/RAG-system faktisk udtrække et rent faktum fra denne beskrivelse." Tynd, adjektivtung tekst scorer lavere, selv med perfekt schema.org-markup.
- **`llms.txt`**: genererer en reel, standardkompatibel `llms.txt`-fil, der opsummerer dit katalog til AI-systemer, leveret på din butiks reelle rod (`/llms.txt`) — ikke gemt under en app-proxy-sti, hvor crawlere ikke finder den.
- **`agents.md`**: genererer en fil, der beskriver din butik til autonome shopping-agenter — varianter, søgning, checkout — udelukkende bygget på reelle data, din butik allerede eksponerer, intet opfundet.
- **Organization-schema**: publicerer dine virksomhedsoplysninger (juridisk navn, moms-/CVR-nummer, adresse) som strukturerede data, så AI-motorer kan verificere, at du er en reel, ansvarlig virksomhed, før de anbefaler dig.

På Free dækker audits dine første 20 produkter, engangs, uden historik. Grow og Unlimited scanner hele dit katalog og gemmer hver tidligere scanning til trendsammenligning.

## 4. Crawler AI

Vælg et produkt, og appen henter dets side præcis, som en AI-crawler gør — ingen JavaScript-udførelse, ligesom GPTBot, ClaudeBot eller PerplexityBot — så du ser præcis, hvad der er synligt for disse motorer: om din `robots.txt` blokerer dem (tjekket pr. bot, ikke bare en generisk tilladt/afvist), og om dine strukturerede data faktisk overlever i den rå HTML, disse bots læser.

**Konkurrentsammenligning** (egen fane fra denne side): indsæt en konkurrents produkt-URL, og få de samme GEO-signaler sammenlignet side om side med dine egne — samme slags forskel, du ville få fra en manuel audit, uden at skulle tilmelde dig konkurrentens egne værktøjer.

## 5. FAQ product

På Grow eller Unlimited vælger du et produkt og klikker på **Generate FAQs** for tre til fem spørgsmål-og-svar-par, der udelukkende er udkast baseret på produktets reelle titel, beskrivelse, leverandør og specifikationer — modellen er eksplicit instrueret i aldrig at tilføje en detalje, der ikke allerede findes i dine data. Gennemgå hvert udkast; intet publiceres uden din udtrykkelige **Approve**. Godkendte FAQ'er vises på den live produktside og markeres op som `FAQPage`-strukturerede data, så de både er læsbare for mennesker og citérbare for maskiner.

**Omskrivning af indhold** (egen fane fra denne side): appen kan omskrive en produktbeskrivelse, så den bliver tættere på verificerbare fakta og lettere for en generativ motor at citere — du ser altid en før/efter-sammenligning og godkender, før noget skrives tilbage til produktet.

## 6. Link Coach

Analyserer hvor godt dine produkter er forbundet med hinanden gennem fælles kollektioner, leverandører og tags — intern linking er et signal, AI-systemer bruger til at forstå, hvad dit katalog dækker som helhed, ikke kun én side ad gangen. Viser forældreløse produkter uden meningsfulde forbindelser og forklarlige forslag til at rette det.

## 7. Visibility AI

Tilføj op til en håndfuld prompts, du realistisk ville forvente, at en kunde stiller en AI-assistent (grænsen afhænger af din plan — se Pricing nedenfor), og hver uge tjekker appen, om Claude, ChatGPT, Gemini og Perplexity nævner din butik i svaret, sporet over tid pr. motor. På Grow og Unlimited viser dette også, hvordan du sammenlignes med navngivne konkurrenter på de samme prompts.

**AI-henvisningstrafik** (Grow og Unlimited): en let, privatlivsrespekterende pixel registrerer, når et besøg på storefronten faktisk stammer fra en af disse AI-motorer (via referrer, kun efter at besøgende har givet analysesamtykke gennem din butiks cookiebanner) og rapporterer, hvor mange sådanne besøg du fik i de sidste 7 dage — den anden halvdel af loopet, som visibility-sporing alene ikke kan vise: ikke kun "bliver vi nævnt," men "sender den omtale nogen."

## 8. Support

En AI-chatassistent findes i appen (ikon nederst til højre) til spørgsmål om GEO, dine auditresultater, eller hvordan en bestemt funktion virker. Hvis den ikke kan hjælpe, kan du bede om at tale med et menneske, og samtalen videresendes direkte til IFG eCommerce.

## 9. Settings

Her administrerer du svarene fra opsætningsguiden (politikker, virksomhedsdata, grænsefladesprog — skift øjeblikkeligt mellem 30 sprog, uden genindlæsningsforsinkelse), gentjekker aktiveringen af temaembedden og ser din kontos Shopify-scopes.

## 10. Pricing

**Pricing** viser Free, Grow og Unlimited side om side, månedligt eller årligt (årligt er cirka 2 måneder gratis på begge betalte niveauer). Du kan opgradere, nedgradere eller vende tilbage til Free når som helst, direkte fra appen — ingen e-mail nødvendig. Se [FAQ](faq.html) for nøjagtige plangrænser.

Det er hele loopet. De fleste forhandlere kører en audit igen efter at have tilføjet nye produkter, tjekker crawler-simulatoren, når de opdaterer en beskrivelse, og kigger på Dashboardets Readiness Matrix ugentligt.

[← Tilbage til Hjælpecenter](index.html)
