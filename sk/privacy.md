---
title: IFG GEO Optimizer
description: Dokumentácia, časté otázky a právne stránky pre Shopify aplikáciu IFG GEO Optimizer.
lang: sk
---

# Zásady ochrany osobných údajov

<div class="lang-switcher">
{% include lang-switcher.html current="sk" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify aplikácia pre Generative Engine Optimization
Posledná aktualizácia: júl 2026

## 1. Prevádzkovateľ údajov

Prevádzkovateľom osobných údajov spracúvaných prostredníctvom aplikácie **IFG GEO Optimizer** je:

**IFG eCommerce** — so sídlom v Ríme, Taliansko
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Čo zbierame

- **Údaje o účte obchodníka (cez Shopify OAuth)**: doménu vášho obchodu, prístupový token API a e-mailovú adresu priradenú k vášmu účtu Shopify.
- **Dáta katalógu (iba na čítanie)**: názvy produktov, popisy, výrobcu, ceny, možnosti a technické parametre — používané na spúšťanie auditov, simuláciu správania crawlerov, hodnotenie extrahovateľnosti obsahu a tvorbu návrhov FAQ alebo prepísaných popisov.
- **Konfigurácia obchodu**: váš aktívny plán, podrobnosti o reklamačnej a dopravnej politike a firemné údaje, ktoré zadáte v Nastaveniach, uložené audity, návrhy FAQ a prepísaného obsahu a prompty, ktoré si zvolíte sledovať pre viditeľnosť AI.
- **Správy podpory v chate**: text, ktorý si vymieňate s AI asistentom v aplikácii, vrátane prepisu konverzácie postúpeného nám, ak výslovne požiadate o rozhovor s človekom.
- **Anonymná návštevnosť storefrontu (Web Pixel, Grow/Unlimited)**: keď návštevník príde na stránku produktu z rozpoznaného AI systému (ChatGPT, Perplexity, Claude, Gemini, Copilot), zaznamenáme systém, URL adresu stránky a časovú pečiatku — iba ak návštevník už udelil súhlas s analytikou cez cookie lištu vášho obchodu. Nezbiera sa žiadny identifikátor návštevníka, cookie ani dáta o relácii.
- **Technické dáta**: časové pečiatky požiadaviek, interné identifikátory záznamov a systémové logy.

> Aplikácia **nikdy nežiada ani nedostáva osobné dáta koncových zákazníkov** — žiadne mená, e-maily, adresy ani objednávky. Požadované oprávnenia Shopify sú `read_products`, `write_products` (katalóg a štruktúrované dáta), `read_themes` (kontrola aktivácie embedu témy) a `write_pixels` (aktivácia vyššie uvedeného anonymného pixelu návštevnosti).

## 3. Prečo ich spracúvame a na akom právnom základe

Tieto dáta spracúvame na poskytovanie služby, kvôli ktorej ste si aplikáciu nainštalovali — podľa čl. 6 ods. 1 písm. b) GDPR, plnenie zmluvy: analýza a zlepšovanie viditeľnosti vášho katalógu na generatívnych vyhľadávacích systémoch, vrátane AI-asistovaného tvorby FAQ a prepisovania obsahu, chatu podpory v aplikácii, týždenného sledovania AI viditeľnosti na promptoch, ktoré si zvolíte, a merania anonymnej návštevnosti z AI referrerov — všetko buď iniciované obchodníkom, alebo v prípade pixelu návštevnosti podmienené súhlasom na vašom storefronte.

## 4. Ako ich zbierame

Údaje o účte sa zbierajú raz, prostredníctvom Shopify OAuth procesu, pri inštalácii. Dáta katalógu sa čítajú cez Shopify Admin API iba vtedy, keď na dashboarde spustíte akciu. Pixel návštevnosti beží na vašom storefronte a hlási udalosti iba po udelení súhlasu; nič iné na pozadí nebeží bez toho, aby ste si to vyžiadali.

## 5. S kým ich zdieľame

- **Google Firebase / Cloud Firestore** — ukladá vašu konfiguráciu, relácie a návrhy. Google LLC (USA) sa zúčastňuje na rámci EU-US Data Privacy Framework. Dáta sú uložené v regióne europe-west1 (Belgicko).
- **Anthropic PBC (USA)** — poskytuje model Claude používaný na tvorbu FAQ, prepisovanie obsahu a chat podpory v aplikácii, iba na základe vašej výslovnej akcie. Dostáva iba atribúty produktu alebo text chatu, ktoré poskytnete — nikdy dáta zákazníkov.
- **OpenAI, Inc. (USA)** a **Perplexity AI, Inc. (USA)** — používané výlučne na týždenné sledovanie AI viditeľnosti pri promptoch, ktoré si výslovne zvolíte sledovať. Dostávajú iba text sledovaného promptu — nikdy dáta zákazníkov.
- **Google LLC (USA)** — poskytuje model Gemini, používaný rovnakým spôsobom ako OpenAI/Perplexity vyššie pri sledovaní viditeľnosti (odlišné použitie od Firebase/Firestore, ktoré slúži iba na ukladanie).
- **Resend, Inc. (USA)** — posiela nám oznámenie s názvom obchodu a prepisom konverzácie z chatu podpory, iba keď výslovne požiadate o rozhovor s človekom v chate podpory.
- **Shopify Inc.** — samotná platforma a zdroj infraštruktúry Admin API a Web Pixel, ktoré aplikácia používa.

Dáta nepredávame a nepoužívame ich na marketing ani behaviorálne profilovanie.

## 6. Ako dlho ich uchovávame

- **Session tokeny**: spravované životným cyklom offline tokenov Shopify, automaticky obnovované.
- **Konfigurácia, audity, návrhy a udalosti návštevnosti**: uchovávané po celú dobu, kým je aplikácia nainštalovaná. Odinštalovanie spustí webhook Shopify `shop/redact`, ktorý úplne vymaže konfiguráciu a relácie vášho obchodu.
- **Technické logy**: uchovávané podľa štandardnej doby uchovávania logov Google Cloud.

## 7. Vaše práva

Podľa článkov 15 – 22 GDPR môžete požiadať o prístup k vašim údajom, opravu nepresných údajov alebo ich vymazanie — najjednoduchší spôsob je odinštalovanie aplikácie — alebo namietať proti spracúvaniu. Môžete tiež podať sťažnosť na váš miestny úrad na ochranu osobných údajov. Keďže aplikácia nikdy nespracúva osobné dáta koncových zákazníkov, webhooky súladu `customers/data_request` a `customers/redact` odpovedajú potvrdením, že nie je čo exportovať ani vymazať.

## 8. Bezpečnosť

Všetka komunikácia prebieha cez HTTPS/TLS 1.2+. Autentifikačné tokeny Shopify nie sú nikdy vystavené prehliadaču. Každý webhook je pred spracovaním overený kontrolou HMAC SHA-256 v konštantnom čase. Databáza je dostupná iba z backendu, autentifikovaného prostredníctvom vlastnej identity služby hostingovej platformy — v kóde nie sú žiadne statické prihlasovacie údaje a priamy prístup klienta je zamietnutý vlastnými bezpečnostnými pravidlami databázy. Dáta sú šifrované počas prenosu aj v pokoji.

## 9. Zmeny

Tieto zásady môžeme z času na čas aktualizovať. Podstatné zmeny sa premietnu tu, s aktuálnym dátumom hore.

---

**Otázky ohľadom vašich dát?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Späť do Centra pomoci](index.html)
