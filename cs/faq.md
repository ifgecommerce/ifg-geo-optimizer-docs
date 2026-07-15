---
title: IFG GEO Optimizer
description: Dokumentace, FAQ a právní stránky aplikace Shopify IFG GEO Optimizer.
lang: cs
---

# Často kladené otázky

<div class="lang-switcher">
{% include lang-switcher.html current="cs" slug="faq" %}
</div>

**Jaký je rozdíl mezi GEO a SEO?**
Tradiční SEO optimalizuje pro vyhledávače, které řadí a vypisují odkazy. GEO (Generative Engine Optimization) optimalizuje pro AI systémy, které čtou váš obsah a přímo generují odpověď nebo doporučení — ChatGPT, Perplexity, Gemini, Claude a Google AI Overviews. Obě disciplíny se překrývají, ale GEO se zajímá o věci, které klasické SEO nástroje nekontrolují: zda má stránka produktu kompletní strukturovaná data, zda AI crawler dokáže skutečně přečíst váš obsah bez spuštění JavaScriptu, a zda je váš text napsaný tak, aby se snadno citoval.

**Dotýká se aplikace někdy dat mých zákazníků?**
Ne, žádná osobní data zákazníků. Oprávnění aplikace na Shopify jsou `read_products`, `write_products`, `read_themes` a `write_pixels` — čtení a vylepšování vašeho katalogu, kontrola, že je embed šablony aktivní, a aktivace anonymního pixelu návštěvnosti storefrontu (viz níže). Nikdy nežádá o objednávky ani záznamy zákazníků. Kompletní přehled najdete v [Zásadách ochrany osobních údajů](privacy.html).

**Co je pixel návštěvnosti z AI odkazů a sleduje mé zákazníky?**
Na Grow a Unlimited malý Web Pixel detekuje, když návštěva storefrontu přichází ze známého AI enginu (přes referrer prohlížeče), a hlásí engine, stránku a časové razítko — nic, co by identifikovalo návštěvníka, žádné cookies, žádná data o relaci. Spouští se jen tehdy, pokud návštěvník už udělil souhlas s analytikou přes cookie lištu vašeho obchodu (Shopify Customer Privacy API). Používá se k zobrazení dlaždice na Dashboardu („Návštěvnost z AI odkazů, posledních 7 dní") — protějšek ke sledování Visibility AI, které vám řekne, jestli jste zmiňováni, ale ne jestli ta zmínka někoho poslala.

**Co přesně mění tlačítko „Fix" u auditu katalogu?**
Zapisuje chybějící strukturovaná data schema.org do metapole produktu — například technické specifikace odvozené z existujících možností produktu. Nikdy se nedotkne názvu produktu, popisu, obrázků ani ceny a nikdy nevymýšlí data, která nedokáže ověřit: chybějící čárový kód například zůstane chybějící, místo aby byl odhadnut.

**Jsou odpovědi FAQ a přepsané popisy vymyšlené AI, nebo vycházejí z mého reálného produktu?**
Model vidí pouze data produktu, která už máte — název, popis, výrobce a technické specifikace — a má výslovný pokyn nepřidávat nic, co v těchto datech není. Každou FAQ nebo přepsaný popis před publikováním zkontrolujete; nic nejde live automaticky.

**Co se stane s mými daty, když aplikaci odinstaluji?**
Konfigurace vašeho obchodu, uložené audity, návrhy FAQ a přepisů obsahu, sledované prompty pro viditelnost a záznamy o návštěvnosti z AI odkazů se automaticky smažou, jakmile nás Shopify upozorní na odinstalování. Aplikace si po vašem odchodu nic neponechává.

**Mohu zrušit nebo downgradovat bez kontaktování podpory?**
Ano. Jděte v aplikaci na **Pricing** a kdykoliv přepněte na Free — projeví se to okamžitě, bez nutnosti e-mailu.

## Limity plánů

| Funkce | Free | Grow | Unlimited |
|---|---|---|---|
| Audit katalogu | Prvních 20 produktů, jednorázově, bez historie | Celý katalog + historie | Celý katalog + historie |
| Simulátor crawleru | 20/měsíc | 300/měsíc | 1 000/měsíc |
| Porovnání s konkurencí | 10/měsíc | 50/měsíc | 150/měsíc |
| Generování FAQ | Není součástí | 500/měsíc | 500/měsíc |
| Přepis obsahu | Není součástí | 300/měsíc | 300/měsíc |
| Visibility AI (sledované prompty) | Není součástí | 5 promptů | 15 promptů |
| Pixel návštěvnosti z AI odkazů | Není součástí | Součástí | Součástí |
| AI chat podpory | 1 000 zpráv/měsíc | 1 000 zpráv/měsíc | 1 000 zpráv/měsíc |
| Jazyky rozhraní | Všech 30 | Všech 30 | Všech 30 |

Měsíční ceny: Free $0, Grow $9.99, Unlimited $19.99. Roční fakturace na Grow/Unlimited vychází zhruba na dva měsíce zdarma oproti měsíční platbě.

**Proč plán Free pokrývá jen 20 produktů?**
Účelem je nechat vás vidět reálné výsledky na vašem vlastním katalogu, než se zavážete k placenému plánu. Grow a Unlimited tento limit odstraňují a uchovávají kompletní historii minulých auditů.

**Existuje opravdu limit na generování FAQ i na Unlimited?**
Ano — 500 generování měsíčně, záměrně, i na nejvyšším plánu. Udržuje to funkci udržitelnou při současné ceně; pokud máte objemově velký katalog, který potřebuje víc, ozvěte se a domluvíme se.

**Proč je AI chat podpory stejný na každém plánu?**
Je to produktové rozhodnutí, ne opomenutí: asistence je zahrnuta pro každého, nikdy to není placený rozlišovací prvek. Limit zpráv (1 000/měsíc) existuje pouze jako technická pojistka proti zneužití, ne jako reálný limit — žádné legitimní použití se k němu ani nepřiblíží.

**Našel jsem chybu nebo něco vypadá špatně. Komu to mám nahlásit?**
Napište na [info@ifgecommerce.com](mailto:info@ifgecommerce.com), co jste viděli, a pokud můžete, u kterého produktu nebo stránky — obvykle to stačí k rychlému dohledání problému. Můžete také použít AI chat podpory v aplikaci a požádat o rozhovor s člověkem.

[← Zpět do centra nápovědy](index.html)
