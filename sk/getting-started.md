---
title: IFG GEO Optimizer
description: Dokumentácia, časté otázky a právne stránky pre Shopify aplikáciu IFG GEO Optimizer.
lang: sk
---

# Ako začať

<div class="lang-switcher">
{% include lang-switcher.html current="sk" slug="getting-started" %}
</div>

IFG GEO Optimizer má deväť oblastí, všetky dostupné z hornej navigácie po dokončení nastavenia: **Dashboard**, **Audit katalógu**, **Crawler AI**, **FAQ produktu**, **Link Coach**, **Visibility AI**, **Ceny**, **Nastavenia** a **Podpora**. Tento návod ich prevedie v poradí, v akom ich väčšina obchodníkov používa.

## 1. Inštalácia a dokončenie sprievodcu nastavením

Pri prvom otvorení krátky sprievodca nastavením (asi 2 minúty) zozbiera základné údaje: jazyk rozhrania, podrobnosti o vašej reklamačnej a dopravnej politike, informácie o vašej firme a — jediný krok, ktorý má skutočný technický význam — aktiváciu app embedu **GEO Schema** v editore témy. Nič z toho, čo aplikácia robí neskôr, sa nedostane na váš storefront, kým tento embed nie je zapnutý, takže sa oplatí ho nevynechať. Ktorúkoľvek z týchto odpovedí môžete kedykoľvek zmeniť neskôr v **Nastaveniach**.

## 2. Dashboard

Vaša domovská základňa. Zobrazuje aktuálne GEO skóre (z posledného auditu), **Readiness Matrix** s ôsmimi signálmi na prvý pohľad — extrahovateľnosť obsahu, schéma Organization, `llms.txt`, `agents.md`, prístup crawlerov, pripravenosť na MCP, pripojenie Link Coach a návštevnosť z AI referrerov — plus prioritizovaný zoznam „oprav toto ako prvé" a počítadlá využitia vášho plánu (generovania FAQ, veľkosť katalógu). Všetko tu vedie priamo na stránku, kde môžete konať.

## 3. Audit katalógu

Kliknutím na **Znova skenovať katalóg** skontrolujete každý produkt oproti deviatim poliam štruktúrovaných dát, ktoré vyhľadávacie systémy hľadajú: obrázok, popis, značka, SKU, GTIN, cena, technické parametre, reklamačná politika a dopravná politika. Produkty pod 80/100 zobrazia presne, čo chýba.

- **Oprava na jedno kliknutie**: tam, kde aplikácia dokáže bezpečne odvodiť chýbajúce dáta (zvyčajne technické parametre z existujúcich možností produktu), uvidíte tlačidlo **Opraviť**, ktoré ich zapíše priamo do štruktúrovaných dát produktu. Pre polia, ktoré aplikácia nedokáže overiť, sa nič nevymýšľa — chýbajúci čiarový kód napríklad zostane chýbajúci, namiesto toho, aby bol vymyslený.
- **Skóre content chunking**: popri kontrole štruktúrovaných dát dostane každý produkt samostatné skóre extrahovateľnosti — nie „je pole prítomné", ale „dokáže si AI/RAG systém z tohto popisu naozaj vytiahnuť čistý fakt". Chudobný, príliš prídavnomennými slovami nabitý text dostane nižšie skóre aj s dokonalým značkovaním schema.org.
- **`llms.txt`**: vygeneruje skutočný, štandardom vyhovujúci súbor `llms.txt`, ktorý zhrnie váš katalóg pre AI systémy, servovaný na skutočnom koreni vášho obchodu (`/llms.txt`), nie skrytý pod cestou app proxy, kde by ho crawlery nenašli.
- **`agents.md`**: vygeneruje súbor popisujúci váš obchod pre autonómne nákupné agenty — varianty, vyhľadávanie, checkout — postavený výlučne na reálnych dátach, ktoré váš obchod už poskytuje, bez ničoho vymysleného.
- **Schéma Organization**: publikuje údaje o vašej firme (obchodné meno, IČ DPH/daňové číslo, adresa) ako štruktúrované dáta, aby si AI systémy mohli overiť, že ste skutočný, dôveryhodný podnik, ešte predtým, než vás odporučia.

V pláne Free pokrýva audit prvých 20 produktov, jednorazovo, bez uchovávania histórie. Grow a Unlimited skenujú celý katalóg a uchovávajú každý predchádzajúci sken na porovnanie trendov.

## 4. Crawler AI

Vyberte produkt a aplikácia načíta jeho stránku presne tak, ako to robí AI crawler — bez vykonávania JavaScriptu, rovnako ako GPTBot, ClaudeBot alebo PerplexityBot — takže presne uvidíte, čo je pre tieto systémy viditeľné: či ich blokuje váš `robots.txt` (kontrolované pre jednotlivé boty, nie iba všeobecné povolenie/zákaz) a či vaše štruktúrované dáta skutočne prežijú v surovom HTML, ktorý tieto boty čítajú.

**Porovnanie s konkurenciou** (samostatná karta na tejto stránke): vložte URL adresu produktu konkurencie a získajte rovnaké GEO signály porovnané vedľa seba s vašimi — rovnaký rozdiel, aký by ste dostali z manuálneho auditu, bez potreby registrácie do vlastných nástrojov konkurencie.

## 5. FAQ produktu

V pláne Grow alebo Unlimited vyberte produkt a kliknite na **Generovať FAQ** pre tri až päť dvojíc otázka-odpoveď, vytvorených výlučne z reálneho názvu, popisu, výrobcu a parametrov daného produktu — model má výslovný pokyn nikdy nepridať detail, ktorý sa už nenachádza vo vašich dátach. Skontrolujte každý návrh; nič sa nezverejní bez vášho výslovného **Schválenia**. Schválené FAQ sa zobrazia na živej stránke produktu a sú označené ako štruktúrované dáta `FAQPage`, takže sú čitateľné pre ľudí aj citovateľné pre stroje.

**Prepísanie obsahu** (samostatná karta na tejto stránke): aplikácia dokáže prepísať popis produktu tak, aby bol hustejší na overiteľné fakty a ľahšie citovateľný pre generatívny systém — vždy vidíte porovnanie pred/po a schvaľujete ho ešte predtým, než sa čokoľvek zapíše späť do produktu.

## 6. Link Coach

Analyzuje, ako dobre sú vaše produkty vzájomne prepojené prostredníctvom zdieľaných kolekcií, výrobcov a tagov — interné prelinkovanie je signál, ktorý AI systémy používajú na pochopenie toho, čo váš katalóg pokrýva ako celok, nielen jednu stránku naraz. Zobrazuje osirelé produkty bez zmysluplných prepojení a vysvetliteľné návrhy, ako to napraviť.

## 7. Visibility AI

Pridajte až niekoľko promptov, ktoré by ste reálne očakávali, že zákazník položí AI asistentovi (limit závisí od vášho plánu — pozri Ceny nižšie), a aplikácia každý týždeň kontroluje, či Claude, ChatGPT, Gemini a Perplexity spomínajú váš obchod v odpovedi, sledované v čase pre každý systém zvlášť. V plánoch Grow a Unlimited toto tiež zobrazuje, ako si stojíte v porovnaní s konkrétne pomenovanou konkurenciou pri rovnakých promptoch.

**Návštevnosť z AI referrerov** (Grow a Unlimited): odľahčený pixel rešpektujúci súkromie zisťuje, kedy návšteva storefrontu skutočne pochádza z jedného z týchto AI systémov (cez referrer, iba po tom, ako návštevník udelil súhlas s analytikou cez cookie lištu vášho obchodu) a hlási, koľko takýchto návštev ste mali za posledných 7 dní — druhá polovica sledovania, ktorú samotné sledovanie viditeľnosti nedokáže ukázať: nielen „sme spomínaní", ale „posiela nám tá zmienka niekoho".

## 8. Podpora

V aplikácii žije AI chatový asistent (ikona vpravo dole) pre otázky o GEO, výsledkoch vášho auditu alebo o tom, ako funguje konkrétna funkcia. Ak nedokáže pomôcť, môžete požiadať o rozhovor s človekom a konverzácia sa presmeruje priamo do IFG eCommerce.

## 9. Nastavenia

Tu spravujete odpovede zo sprievodcu nastavením (politiky, firemné údaje, jazyk rozhrania — okamžité prepínanie medzi 30 jazykmi, bez oneskorenia pri načítaní), znova skontrolujete aktiváciu embedu témy a vidíte oprávnenia Shopify vášho účtu.

## 10. Ceny

**Ceny** zobrazujú Free, Grow a Unlimited vedľa seba, mesačne alebo ročne (ročná platba predstavuje približne 2 mesiace zdarma v oboch platených plánoch). Kedykoľvek môžete plán zvýšiť, znížiť alebo sa vrátiť späť na Free, priamo z aplikácie — bez potreby e-mailu. Presné limity plánov nájdete v [FAQ](faq.html).

To je celý cyklus. Väčšina obchodníkov spustí audit znova po pridaní nových produktov, skontroluje simulátor crawlera vždy, keď aktualizuje popis, a týždenne skontroluje Readiness Matrix na Dashboarde.

[← Späť do Centra pomoci](index.html)
