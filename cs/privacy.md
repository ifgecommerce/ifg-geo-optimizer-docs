---
title: IFG GEO Optimizer
description: Dokumentace, FAQ a právní stránky aplikace Shopify IFG GEO Optimizer.
lang: cs
---

# Zásady ochrany osobních údajů

<div class="lang-switcher">
{% include lang-switcher.html current="cs" slug="privacy" %}
</div>

**IFG GEO Optimizer** — aplikace Shopify pro Generative Engine Optimization
Naposledy aktualizováno: červenec 2026

## 1. Správce údajů

Správcem osobních údajů zpracovávaných prostřednictvím **IFG GEO Optimizer** je:

**IFG eCommerce** — se sídlem v Římě, Itálie
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Co shromažďujeme

- **Údaje účtu obchodníka (přes Shopify OAuth)**: doména vašeho obchodu, přístupový token API a e-mailová adresa přiřazená k vašemu účtu Shopify.
- **Data katalogu (pouze pro čtení)**: názvy produktů, popisy, výrobce, ceny, možnosti a technické specifikace — používané ke spouštění auditů, simulaci chování crawlerů, hodnocení extrahovatelnosti obsahu a vytváření návrhů FAQ nebo přepsaných popisů.
- **Konfigurace obchodu**: váš aktivní plán, údaje o politice vrácení a dopravy a firemní údaje zadané v Settings, uložené audity, návrhy FAQ a přepisů obsahu a prompty, které se rozhodnete sledovat pro viditelnost AI.
- **Zprávy chatu podpory**: text, který si vyměňujete s AI asistentem podpory v aplikaci, včetně přepisu předaného nám, pokud výslovně požádáte o rozhovor s člověkem.
- **Anonymní návštěvnost storefrontu (Web Pixel, Grow/Unlimited)**: když návštěvník přijde na stránku produktu z rozpoznaného AI enginu (ChatGPT, Perplexity, Claude, Gemini, Copilot), zaznamenáme engine, URL stránky a časové razítko — pouze pokud návštěvník už udělil souhlas s analytikou přes cookie lištu vašeho obchodu. Nesbírá se žádný identifikátor návštěvníka, cookie ani data o relaci.
- **Technická data**: časová razítka požadavků, interní identifikátory záznamů a systémové logy.

> Aplikace **nikdy nežádá ani nepřijímá osobní údaje koncových zákazníků** — žádná jména, e-maily, adresy ani objednávky. Požadovaná oprávnění Shopify jsou `read_products`, `write_products` (katalog a strukturovaná data), `read_themes` (kontrola, že je embed šablony aktivní) a `write_pixels` (aktivace výše uvedeného anonymního pixelu návštěvnosti).

## 3. Proč tato data zpracováváme a na jakém právním základě

Tato data zpracováváme, abychom poskytli službu, kvůli které jste aplikaci nainstalovali — podle čl. 6 odst. 1 písm. b) GDPR, plnění smlouvy: analýza a zlepšování viditelnosti vašeho katalogu na generativních vyhledávačích, včetně AI asistovaného návrhu FAQ a přepisu obsahu, chatu podpory v aplikaci, týdenního sledování viditelnosti AI na promptech, které si zvolíte, a měření anonymní návštěvnosti z AI odkazů — vše buď iniciováno obchodníkem, nebo, v případě pixelu návštěvnosti, podmíněno souhlasem na vašem storefrontu.

## 4. Jak tato data shromažďujeme

Údaje o účtu se shromažďují jednorázově, přes OAuth flow Shopify, při instalaci. Data katalogu se čtou přes Admin API Shopify pouze tehdy, když spustíte akci z dashboardu. Pixel návštěvnosti běží na vašem storefrontu a hlásí události až po souhlasu; nic dalšího neběží na pozadí, aniž byste o to požádali.

## 5. S kým je sdílíme

- **Google Firebase / Cloud Firestore** — ukládá vaši konfiguraci, relace a návrhy. Google LLC (USA) se účastní EU-US Data Privacy Framework. Data jsou uložena v regionu europe-west1 (Belgie).
- **Anthropic PBC (USA)** — poskytuje model Claude použitý pro návrh FAQ, přepis obsahu a chat podpory v aplikaci, pouze na váš explicitní pokyn. Přijímá pouze atributy produktu nebo text chatu, které poskytnete — nikdy data zákazníků.
- **OpenAI, Inc. (USA)** a **Perplexity AI, Inc. (USA)** — používány výhradně pro týdenní sledování viditelnosti AI na promptech, které se explicitně rozhodnete sledovat. Přijímají pouze text sledovaného promptu — nikdy data zákazníků.
- **Google LLC (USA)** — poskytuje model Gemini, použitý stejným způsobem jako OpenAI/Perplexity výše pro sledování viditelnosti (odlišné použití od Firebase/Firestore, které slouží pouze k ukládání).
- **Resend, Inc. (USA)** — posílá nám oznámení s názvem obchodu a přepisem chatu podpory, pouze tehdy, když v chatu podpory explicitně požádáte o rozhovor s člověkem.
- **Shopify Inc.** — samotná platforma a zdroj infrastruktury Admin API a Web Pixel, kterou aplikace používá.

Data neprodáváme a nepoužíváme je k marketingu ani behaviorálnímu profilování.

## 6. Jak dlouho je uchováváme

- **Přístupové tokeny relace**: spravovány cyklem offline tokenů Shopify, automaticky rotovány.
- **Konfigurace, audity, návrhy a události návštěvnosti**: uchovávány po dobu, po kterou je aplikace nainstalována. Odinstalování spustí webhook Shopify `shop/redact`, který zcela smaže konfiguraci a relace vašeho obchodu.
- **Technické logy**: uchovávány podle standardní doby uchovávání logů Google Cloud.

## 7. Vaše práva

Podle článků 15–22 GDPR můžete požádat o přístup ke svým datům, opravu nepřesných dat nebo jejich smazání — nejjednodušší způsob je odinstalovat aplikaci — nebo vznést námitku proti zpracování. Můžete také podat stížnost u místního úřadu pro ochranu osobních údajů. Jelikož aplikace nikdy nezpracovává osobní údaje koncových zákazníků, compliance webhooky `customers/data_request` a `customers/redact` odpovídají potvrzením, že není co exportovat ani smazat.

## 8. Bezpečnost

Veškerý provoz probíhá přes HTTPS/TLS 1.2+. Autentizační tokeny Shopify nejsou nikdy vystaveny prohlížeči. Každý webhook je před zpracováním ověřen kontrolou HMAC SHA-256 v konstantním čase. Databáze je dostupná pouze z backendu, autentizovaného vlastní identitou služby hostingové platformy — v kódu nejsou žádné statické přihlašovací údaje a přímý přístup klienta je zamítnut vlastními bezpečnostními pravidly databáze. Data jsou šifrována v klidu i při přenosu.

## 9. Změny

Tyto zásady můžeme čas od času aktualizovat. Podstatné změny se projeví zde, s aktuálním datem v záhlaví.

---

**Otázky ohledně vašich dat?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Zpět do centra nápovědy](index.html)
