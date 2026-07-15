---
title: IFG GEO Optimizer
description: Dokumentácia, časté otázky a právne stránky pre Shopify aplikáciu IFG GEO Optimizer.
lang: sk
---

# Často kladené otázky

<div class="lang-switcher">
{% include lang-switcher.html current="sk" slug="faq" %}
</div>

**Aký je rozdiel medzi GEO a SEO?**
Tradičné SEO optimalizuje pre vyhľadávače, ktoré zoraďujú a zobrazujú zoznamy odkazov. GEO (Generative Engine Optimization) optimalizuje pre AI systémy, ktoré čítajú váš obsah a priamo generujú odpoveď alebo odporúčanie — ChatGPT, Perplexity, Gemini, Claude a Google AI Overviews. Obe disciplíny sa prekrývajú, ale GEO sa zaujíma o veci, ktoré klasické SEO nástroje nekontrolujú: či má stránka produktu kompletné štruktúrované dáta, či dokáže AI crawler skutočne prečítať váš obsah bez vykonávania JavaScriptu, a či je text napísaný tak, aby sa dal ľahko citovať.

**Dotýka sa aplikácia niekedy dát mojich zákazníkov?**
Nie, žiadne osobné dáta zákazníkov. Oprávnenia aplikácie na Shopify sú `read_products`, `write_products`, `read_themes` a `write_pixels` — čítanie a vylepšovanie vášho katalógu, kontrola, či je embed témy aktívny, a aktivácia anonymného pixelu návštevnosti storefrontu (pozri nižšie). Nikdy nežiada objednávky ani záznamy zákazníkov. Úplný prehľad nájdete v [Zásadách ochrany osobných údajov](privacy.html).

**Čo je pixel návštevnosti z AI referrerov a sleduje mojich zákazníkov?**
V plánoch Grow a Unlimited malý Web Pixel zisťuje, kedy návšteva storefrontu prichádza zo známeho AI systému (cez referrer prehliadača) a hlási systém, stránku a časovú pečiatku — nič, čo by identifikovalo návštevníka, žiadne cookies, žiadne dáta o relácii. Funguje iba vtedy, ak návštevník už udelil súhlas s analytikou cez cookie lištu vášho obchodu (Shopify Customer Privacy API). Používa sa na zobrazenie dlaždice na Dashboarde („Návštevnosť z AI referrerov, posledných 7 dní") — doplnok k sledovaniu Visibility AI, ktoré vám povie, či ste spomínaní, ale nie, či táto zmienka niekoho poslala.

**Čo presne zmení tlačidlo „Opraviť" pri audite katalógu?**
Zapíše chýbajúce štruktúrované dáta schema.org do metapoľa produktu — napríklad technické parametre odvodené z existujúcich možností produktu. Nikdy sa nedotkne názvu produktu, popisu, obrázkov ani ceny a nikdy si nevymyslí dáta, ktoré nedokáže overiť: chýbajúci čiarový kód napríklad zostane chýbajúci, namiesto toho, aby bol odhadnutý.

**Sú odpovede FAQ a prepísané popisy vymyslené AI, alebo vychádzajú z môjho skutočného produktu?**
Model vidí iba dáta produktu, ktoré už máte — názov, popis, výrobca a technické parametre — a má výslovný pokyn nepridávať nič, čo v týchto dátach nie je. Každé FAQ alebo prepísaný popis skontrolujete pred zverejnením; nič sa nepublikuje automaticky.

**Čo sa stane s mojimi dátami, ak aplikáciu odinštalujem?**
Konfigurácia vášho obchodu, uložené audity, návrhy FAQ a prepísaného obsahu, prompty pre sledovanie viditeľnosti a udalosti návštevnosti z AI referrerov sa automaticky vymažú, keď nám Shopify oznámi odinštaláciu. Aplikácia si po vašom odchode nič neponecháva.

**Môžem zrušiť alebo znížiť plán bez kontaktovania podpory?**
Áno. Choďte do sekcie **Ceny** v aplikácii a kedykoľvek prepnite na Free — zmena sa prejaví okamžite, bez potreby e-mailu.

## Limity plánov

| Funkcia | Free | Grow | Unlimited |
|---|---|---|---|
| Audit katalógu | Prvých 20 produktov, jednorazovo, bez histórie | Celý katalóg + história | Celý katalóg + história |
| Simulátor crawlera | 20/mesiac | 300/mesiac | 1 000/mesiac |
| Porovnanie s konkurenciou | 10/mesiac | 50/mesiac | 150/mesiac |
| Generovanie FAQ | Nie je súčasťou | 500/mesiac | 500/mesiac |
| Prepísanie obsahu | Nie je súčasťou | 300/mesiac | 300/mesiac |
| Visibility AI (sledované prompty) | Nie je súčasťou | 5 promptov | 15 promptov |
| Pixel návštevnosti z AI referrerov | Nie je súčasťou | Zahrnuté | Zahrnuté |
| AI chat podpory | 1 000 správ/mesiac | 1 000 správ/mesiac | 1 000 správ/mesiac |
| Jazyky rozhrania | Všetkých 30 | Všetkých 30 | Všetkých 30 |

Mesačné ceny: Free $0, Grow $9.99, Unlimited $19.99. Ročná fakturácia pri Grow/Unlimited predstavuje približne dva mesiace zdarma v porovnaní s mesačnou platbou.

**Prečo plán Free pokrýva iba 20 produktov?**
Cieľom je umožniť vám vidieť reálne výsledky na vlastnom katalógu ešte pred prechodom na platený plán. Grow a Unlimited odstraňujú tento limit a uchovávajú kompletnú históriu predchádzajúcich auditov.

**Existuje naozaj limit na generovanie FAQ aj v pláne Unlimited?**
Áno — 500 generovaní mesačne, zámerne, aj v najvyššom pláne. Udržiava to funkciu udržateľnú pri súčasnej cene; ak máte katalóg s vysokým objemom a potrebujete viac, ozvite sa nám a nájdeme riešenie.

**Prečo je AI chat podpory rovnaký vo všetkých plánoch?**
Je to produktové rozhodnutie, nie prehliadnutie: podpora je zahrnutá pre všetkých, nikdy nie je plateným rozlišovacím prvkom. Limit správ (1 000/mesiac) existuje iba ako technická poistka proti zneužitiu, nie ako reálne obmedzenie — žiadne legitímne použitie sa k nemu ani nepribližuje.

**Našiel som chybu alebo niečo nevyzerá správne. Komu to mám nahlásiť?**
Napíšte na [info@ifgecommerce.com](mailto:info@ifgecommerce.com) s popisom toho, čo ste videli, a ak viete, aj s uvedením produktu alebo stránky — to zvyčajne stačí na rýchle vyriešenie problému. Môžete tiež použiť AI chat podpory priamo v aplikácii a požiadať o rozhovor s človekom.

[← Späť do Centra pomoci](index.html)
