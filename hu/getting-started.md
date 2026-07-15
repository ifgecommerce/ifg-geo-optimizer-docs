---
title: IFG GEO Optimizer
description: Dokumentáció, GYIK és jogi oldalak az IFG GEO Optimizer Shopify alkalmazáshoz.
lang: hu
---

# Kezdő lépések

<div class="lang-switcher">
{% include lang-switcher.html current="hu" slug="getting-started" %}
</div>

Az IFG GEO Optimizer kilenc területet tartalmaz, amelyek a beállítás befejezése után mind elérhetők a felső navigációból: **Vezérlőpult**, **Katalógus audit**, **Crawler AI**, **FAQ termék**, **Link Coach**, **Visibility AI**, **Árazás**, **Beállítások** és **Támogatás**. Ez az útmutató sorra végigveszi mindegyiket, abban a sorrendben, ahogy a legtöbb kereskedő használja őket.

## 1. Telepítés és a beállítási varázsló elvégzése

Az első megnyitáskor egy rövid, irányított beállítás (kb. 2 perc) összegyűjti az alapokat: a felület nyelvét, a visszaküldési és szállítási szabályzatod adatait, a cégadataidat, valamint — az egyetlen lépés, ami technikailag valóban számít — a **GEO Schema** app embed aktiválását a téma szerkesztőjében. Amíg ez az embed nincs bekapcsolva, az alkalmazás semmilyen későbbi művelete nem jut el a webáruházad frontendjére, ezért érdemes ezt a lépést nem kihagyni. Ezeket a válaszokat bármikor módosíthatod később a **Beállítások** menüben.

## 2. Vezérlőpult

Ez a kiindulópontod. Megmutatja az aktuális GEO pontszámodat (az utolsó audit alapján), egy **Readiness Matrix**-ot nyolc, egy pillantásra átlátható jelzővel — tartalom kinyerhetősége, Organization schema, `llms.txt`, `agents.md`, crawler hozzáférés, MCP-készenlét, Link Coach kapcsolódás és AI-eredetű forgalom —, valamint egy priorizált "ezt javítsd először" listát és a csomagod használati számlálóit (FAQ generálások, katalógus mérete). Innen minden egyenesen arra az oldalra vezet, ahol cselekedni tudsz.

## 3. Katalógus audit

Kattints a **Katalógus újraellenőrzése** gombra, hogy minden terméket ellenőrizz kilenc olyan strukturáltadat-mező alapján, amelyeket a keresőmotorok keresnek: kép, leírás, márka, SKU, GTIN, ár, műszaki specifikáció, visszaküldési szabályzat és szállítási szabályzat. A 80/100 alatti termékek pontosan megmutatják, mi hiányzik.

- **Egy kattintásos javítás**: ahol az alkalmazás biztonságosan tudja levezetni a hiányzó adatot (jellemzően a műszaki specifikációkat a meglévő termékopciókból), egy **Javítás** gomb jelenik meg, amely közvetlenül beírja azt a termék strukturált adataiba. Semmit nem találunk ki azoknál a mezőknél, amelyeket az alkalmazás nem tud ellenőrizni — egy hiányzó vonalkód például hiányzó marad, ahelyett hogy kitalálnánk.
- **Content chunking pontszám**: a strukturáltadat-ellenőrzés mellett minden termék kap egy külön kinyerhetőségi pontszámot is — nem azt nézi, hogy "jelen van-e a mező", hanem hogy "tud-e egy AI/RAG rendszer valóban tiszta tényt kinyerni ebből a leírásból". A gyenge, jelzős, tartalom nélküli szöveg alacsonyabb pontszámot kap még tökéletes schema.org markup mellett is.
- **`llms.txt`**: valódi, szabványoknak megfelelő `llms.txt` fájlt generál, amely összefoglalja a katalógusodat az AI rendszerek számára, és a bolt valódi gyökerén (`/llms.txt`) érhető el, nem egy app proxy útvonal alá temetve, ahol a crawlerek nem találnák meg.
- **`agents.md`**: olyan fájlt generál, amely a boltodat írja le az autonóm vásárlási ügynökök számára — variánsok, keresés, checkout —, kizárólag olyan valós adatokból építve, amelyeket a bolt már amúgy is publikál, semmi kitalált.
- **Organization schema**: közzéteszi a céged adatait (cégnév, adószám/áfa-szám, cím) strukturált adatként, hogy az AI motorok ellenőrizhessék, valódi, elszámoltatható vállalkozásról van szó, mielőtt ajánlanának.

Free csomagon az audit az első 20 terméket fedi le, egyszeri alkalommal, előzmények nélkül. Grow és Unlimited csomagon a teljes katalógus átvizsgálásra kerül, és minden korábbi vizsgálat megmarad a trendösszehasonlításhoz.

## 4. Crawler AI

Válassz ki egy terméket, és az alkalmazás pontosan úgy tölti le az oldalát, ahogy egy AI crawler tenné — JavaScript-végrehajtás nélkül, ugyanúgy, mint a GPTBot, a ClaudeBot vagy a PerplexityBot —, így pontosan látod, mi az, ami ezen motorok számára látható: blokkolja-e a `robots.txt` (botonként ellenőrizve, nem csak egy általános engedélyezés/tiltás alapján), és hogy a strukturált adataid valóban megmaradnak-e a nyers HTML-ben, amit ezek a botok olvasnak.

**Versenytárs-összehasonlítás** (saját fül ezen az oldalon): illeszd be egy versenytárs termék-URL-jét, és ugyanazokat a GEO jelzőket kapod meg egymás mellett összehasonlítva a sajátoddal — ugyanaz a fajta különbség, amit egy kézi audittal kapnál, anélkül hogy regisztrálnod kellene a versenytárs saját eszközeire.

## 5. FAQ termék

Grow vagy Unlimited csomagon válassz ki egy terméket, és kattints a **FAQ generálása** gombra három-öt kérdés-válasz párért, amelyeket kizárólag az adott termék valódi címéből, leírásából, gyártójából és specifikációiból állít össze a modell — a modell kifejezett utasítást kap arra, hogy soha ne adjon hozzá olyan részletet, ami még nincs az adataid között. Nézz át minden tervezetet; semmi nem jelenik meg a te kifejezett **Jóváhagyásod** nélkül. A jóváhagyott FAQ-k megjelennek az élő termékoldalon, és `FAQPage` strukturált adatként vannak megjelölve, így egyszerre olvashatók emberek számára és idézhetők gépek által.

**Tartalom átírása** (saját fül ezen az oldalon): az alkalmazás képes átírni egy termékleírást úgy, hogy sűrűbben tartalmazzon ellenőrizhető tényeket, és könnyebben idézhető legyen egy generatív motor számára — mindig látod az előtte/utána összehasonlítást, és jóvá kell hagynod, mielőtt bármi visszaírásra kerülne a termékbe.

## 6. Link Coach

Elemzi, mennyire jól kapcsolódnak egymáshoz a termékeid közös kollekciókon, gyártókon és címkéken keresztül — a belső linkelés olyan jelzés, amelyet az AI rendszerek arra használnak, hogy megértsék, mit fed le a katalógusod egészében, nem csak egy-egy oldalt külön-külön. Megmutatja az árva termékeket, amelyeknek nincs érdemi kapcsolódásuk, és magyarázattal ellátott javaslatokat ad ennek javítására.

## 7. Visibility AI

Adj hozzá néhány olyan promptot, amelyet reálisan elvárhatnál, hogy egy vásárló feltegyen egy AI asszisztensnek (a limit a csomagodtól függ — lásd az Árazás részt alább), és az alkalmazás hetente ellenőrzi, hogy a Claude, ChatGPT, Gemini és Perplexity megemlíti-e a boltodat a válaszban, motoronként időben követve. Grow és Unlimited csomagon ez azt is megmutatja, hogyan viszonyulsz megnevezett versenytársakhoz ugyanazokon a promptokon.

**AI-eredetű forgalom** (Grow és Unlimited): egy könnyű, adatvédelmet tiszteletben tartó pixel érzékeli, amikor egy webáruház-látogatás ténylegesen az egyik ilyen AI motorból származik (a referrer alapján, csak azután, hogy a látogató hozzájárult az analitikai adatgyűjtéshez a bolt cookie-bannerén keresztül), és jelenti, hány ilyen látogatásod volt az elmúlt 7 napban — ez a kör második fele, amit önmagában a visibility tracking nem tud megmutatni: nem csak azt, hogy "megemlítenek-e minket", hanem hogy "az a megemlítés küld-e valakit hozzánk".

## 8. Támogatás

Egy AI chat asszisztens él az alkalmazásban (jobb alsó ikon) a GEO-val, az audit eredményeivel vagy egy adott funkció működésével kapcsolatos kérdésekhez. Ha nem tud segíteni, kérheted, hogy emberrel beszélhess, és a beszélgetés közvetlenül továbbításra kerül az IFG eCommerce felé.

## 9. Beállítások

Itt kezelheted a beállítási varázsló válaszait (szabályzatok, cégadatok, felület nyelve — azonnal válthatsz a 30 nyelv között, újratöltési késleltetés nélkül), újraellenőrizheted a téma embed aktiválását, és megnézheted a fiókod Shopify jogosultsági köreit (scope-jait).

## 10. Árazás

Az **Árazás** oldal egymás mellett mutatja a Free, Grow és Unlimited csomagokat, havi vagy éves bontásban (az éves fizetés a két fizetős csomagon nagyjából 2 hónapnyi kedvezményt jelent). Bármikor válthatsz csomagot felfelé, lefelé, vagy visszaválthatsz Free-re, közvetlenül az alkalmazásból — e-mail nélkül. A pontos csomaghatárokért lásd a [GYIK](faq.html) oldalt.

Ez a teljes ciklus. A legtöbb kereskedő új termékek hozzáadása után újra lefuttatja az auditot, minden leírás-frissítés után megnézi a crawler szimulátort, és hetente rápillant a Vezérlőpult Readiness Matrixára.

[← Vissza a Súgóközponthoz](index.html)
