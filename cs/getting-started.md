---
title: IFG GEO Optimizer
description: Dokumentace, FAQ a právní stránky aplikace Shopify IFG GEO Optimizer.
lang: cs
---

# Začínáme

<div class="lang-switcher">
{% include lang-switcher.html current="cs" slug="getting-started" %}
</div>

IFG GEO Optimizer má devět oblastí, všechny dostupné z horní navigace po dokončení nastavení: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** a **Support**. Tento průvodce projde všemi v pořadí, ve kterém je většina obchodníků používá.

## 1. Instalace a dokončení průvodce nastavením

Při prvním otevření vás krátký asistovaný setup (asi 2 minuty) provede základy: jazyk rozhraní, údaje o vaší politice vrácení zboží a dopravy, informace o vaší firmě a — jediný krok, který je technicky opravdu důležitý — aktivace app embedu **GEO Schema** v editoru šablony. Dokud tento embed nezapnete, nic z toho, co aplikace dělá poté, se neprojeví na vašem storefrontu, takže tento krok se vyplatí nepřeskočit. Kteroukoliv z těchto odpovědí můžete kdykoliv později změnit v **Settings**.

## 2. Dashboard

Vaše výchozí obrazovka. Zobrazuje aktuální GEO skóre (z posledního auditu), **Readiness Matrix** s osmi signály na první pohled — extrahovatelnost obsahu, schéma Organization, `llms.txt`, `agents.md`, přístup crawlerů, připravenost MCP, propojenost Link Coach a návštěvnost z AI odkazů — plus prioritizovaný seznam „opravit nejdřív" a počítadla využití vašeho plánu (generování FAQ, velikost katalogu). Vše zde vede přímo na stránku, kde s tím můžete pracovat.

## 3. Audit catalog

Klikněte na **Rescan catalog** a zkontrolujte každý produkt podle devíti polí strukturovaných dat, která vyhledávače hledají: obrázek, popis, značka, SKU, GTIN, cena, technické specifikace, politika vrácení a politika dopravy. Produkty pod 80/100 zobrazí přesně, co chybí.

- **Oprava na jedno kliknutí**: tam, kde aplikace dokáže bezpečně odvodit chybějící data (obvykle technické specifikace z existujících možností produktu), uvidíte tlačítko **Fix**, které je zapíše přímo do strukturovaných dat produktu. U polí, která aplikace nedokáže ověřit, se nic nevymýšlí — chybějící čárový kód například zůstane chybějící, místo aby byl odhadnut.
- **Content chunking score**: vedle kontroly strukturovaných dat získá každý produkt samostatné skóre extrahovatelnosti — nejde o „je pole přítomné", ale o to, „dokáže AI/RAG systém z tohoto popisu skutečně vytáhnout čistý fakt". Řídký text plný přídavných jmen skóruje hůř i s dokonalým markupem schema.org.
- **`llms.txt`**: generuje skutečný, standardům odpovídající soubor `llms.txt` shrnující váš katalog pro AI systémy, servírovaný na skutečném kořeni vašeho obchodu (`/llms.txt`), ne schovaný pod cestou app proxy, kde by ho crawlery nenašly.
- **`agents.md`**: generuje soubor popisující váš obchod autonomním nákupním agentům — varianty, vyhledávání, checkout — postavený pouze na reálných datech, která váš obchod už zveřejňuje, nic vymyšleného.
- **Schéma Organization**: publikuje údaje vaší firmy (oficiální název, DIČ/IČO, adresu) jako strukturovaná data, aby AI enginy mohly ověřit, že jste skutečná, důvěryhodná firma, než vás doporučí.

Na plánu Free pokrývají audity prvních 20 produktů, jednorázově, bez uchovávané historie. Grow a Unlimited prohledávají celý katalog a uchovávají historii každého předchozího skenu pro srovnání trendů.

## 4. Crawler AI

Vyberte produkt a aplikace načte jeho stránku přesně tak, jak to dělá AI crawler — bez spuštění JavaScriptu, stejně jako GPTBot, ClaudeBot nebo PerplexityBot — takže přesně vidíte, co je pro tyto enginy viditelné: zda je blokuje váš `robots.txt` (kontrolováno pro každého bota zvlášť, ne jen obecné povolit/zakázat) a zda strukturovaná data skutečně přežijí v surovém HTML, které tito boti čtou.

**Porovnání s konkurencí** (samostatná záložka na této stránce): vložte URL produktu konkurenta a získáte stejné signály GEO porovnané vedle sebe s vašimi — stejný typ rozdílu, jaký byste dostali z manuálního auditu, bez nutnosti registrace do nástrojů konkurence.

## 5. FAQ product

Na plánu Grow nebo Unlimited vyberte produkt a klikněte na **Generate FAQs** — vytvoří se tři až pět dvojic otázka-odpověď, sestavených výhradně z reálného názvu, popisu, výrobce a specifikací daného produktu — model má výslovný pokyn nikdy nepřidávat detail, který už není v datech. Zkontrolujte každý návrh; nic se nepublikuje bez vašeho explicitního **Approve**. Schválené FAQ se zobrazí na živé stránce produktu a jsou označkovány jako strukturovaná data `FAQPage`, takže jsou čitelné jak pro lidi, tak citovatelné pro stroje.

**Přepis obsahu** (samostatná záložka na této stránce): aplikace dokáže přepsat popis produktu tak, aby byl hutnější na ověřitelná fakta a snáze citovatelný generativním enginem — vždy vidíte srovnání před/po a schvalujete, než se cokoliv zapíše zpět do produktu.

## 6. Link Coach

Analyzuje, jak dobře jsou vaše produkty vzájemně propojeny přes sdílené kolekce, výrobce a tagy — vnitřní prolinkování je signál, který AI systémy používají k pochopení toho, co váš katalog pokrývá jako celek, ne jen jedna stránka najednou. Zobrazuje osiřelé produkty bez smysluplných propojení a vysvětlené návrhy, jak to napravit.

## 7. Visibility AI

Přidejte až hrstku promptů, na které by se podle vás reálně mohl zákazník zeptat AI asistenta (limit závisí na vašem plánu — viz Pricing níže), a každý týden aplikace zkontroluje, zda Claude, ChatGPT, Gemini a Perplexity zmiňují váš obchod v odpovědi, sledováno v čase pro každý engine zvlášť. Na Grow a Unlimited to navíc ukazuje, jak si stojíte oproti jmenovaným konkurentům na stejných promptech.

**Návštěvnost z AI odkazů** (Grow a Unlimited): odlehčený pixel respektující soukromí detekuje, když návštěva storefrontu skutečně pochází z jednoho z těchto AI enginů (přes referrer, pouze po udělení souhlasu s analytikou návštěvníkem přes cookie lištu vašeho obchodu) a hlásí, kolik takových návštěv jste měli za posledních 7 dní — druhá polovina smyčky, kterou samotné sledování viditelnosti nedokáže ukázat: nejen „jsme zmiňováni", ale „posílá nám ta zmínka někoho".

## 8. Support

V aplikaci žije AI chatový asistent (ikona vpravo dole) pro otázky o GEO, výsledcích vašeho auditu nebo o tom, jak funguje konkrétní funkce. Pokud nedokáže pomoci, můžete požádat o rozhovor s člověkem a konverzace bude přeposlána přímo IFG eCommerce.

## 9. Settings

Zde spravujete odpovědi ze setup wizardu (politiky, firemní údaje, jazyk rozhraní — přepínejte okamžitě mezi 30 jazyky, bez zpoždění při načítání), znovu ověřujete aktivaci embedu šablony a vidíte scopy Shopify vašeho účtu.

## 10. Pricing

**Pricing** zobrazuje Free, Grow a Unlimited vedle sebe, měsíčně nebo ročně (roční platba znamená zhruba 2 měsíce zdarma u obou placených úrovní). Kdykoliv můžete upgradovat, downgradovat nebo se vrátit zpět na Free přímo v aplikaci — bez nutnosti e-mailu. Přesné limity plánů najdete v [FAQ](faq.html).

To je celý cyklus. Většina obchodníků znovu spustí audit po přidání nových produktů, kontroluje simulátor crawleru vždy, když aktualizuje popis, a jednou týdně mrkne na Readiness Matrix na Dashboardu.

[← Zpět do centra nápovědy](index.html)
