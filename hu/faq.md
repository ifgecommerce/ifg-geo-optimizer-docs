---
title: IFG GEO Optimizer
description: Dokumentáció, GYIK és jogi oldalak az IFG GEO Optimizer Shopify alkalmazáshoz.
lang: hu
---

# Gyakran Ismételt Kérdések

<div class="lang-switcher">
{% include lang-switcher.html current="hu" slug="faq" %}
</div>

**Mi a különbség a GEO és a SEO között?**
A hagyományos SEO azoknak a keresőmotoroknak optimizál, amelyek linkeket rangsorolnak és listáznak. A GEO (Generative Engine Optimization) azoknak az AI rendszereknek optimizál, amelyek elolvassák a tartalmadat, és közvetlenül generálnak választ vagy ajánlást — ChatGPT, Perplexity, Gemini, Claude és Google AI Overviews. A kettő átfedésben van, de a GEO olyan dolgokra figyel, amelyeket a klasszikus SEO eszközök nem ellenőriznek: hogy a termékoldaladon teljes-e a strukturált adat, hogy egy AI crawler valóban el tudja-e olvasni a tartalmadat JavaScript futtatása nélkül, és hogy a szöveged olyan-e, amelyet könnyű idézni és hivatkozni.

**Az alkalmazás hozzáfér valaha az ügyfeleim adataihoz?**
Nem, semmilyen személyes ügyféladathoz. Az alkalmazás Shopify jogosultságai `read_products`, `write_products`, `read_themes` és `write_pixels` — a katalógusod olvasása és javítása, a téma embed aktív állapotának ellenőrzése, valamint egy anonim, webáruház-forgalmat mérő pixel aktiválása (lásd lentebb). Soha nem kér hozzáférést rendelésekhez vagy ügyféladatokhoz. A teljes részletekért lásd az [Adatvédelmi szabályzatot](privacy.html).

**Mi az AI-eredetű forgalom pixel, és nyomon követi az ügyfeleimet?**
Grow és Unlimited csomagon egy kis Web Pixel érzékeli, amikor egy webáruház-látogatás egy ismert AI motorból érkezik (a böngésző referrer-je alapján), és jelenti a motort, az oldalt és egy időbélyeget — semmi olyat, ami azonosítaná a látogatót, nincs cookie, nincs munkamenet-adat. Csak akkor fut, ha a látogató már hozzájárult az analitikai adatgyűjtéshez a bolt cookie-bannerén keresztül (Shopify Customer Privacy API). Ezt egy Vezérlőpult csempe megjelenítésére használjuk ("AI-eredetű forgalom, elmúlt 7 nap") — ez a Visibility AI tracking párja, amely azt mutatja meg, hogy megemlítenek-e, de nem azt, hogy az a megemlítés küld-e valakit hozzád.

**Mit változtat valójában a "Javítás" gomb a katalógus auditban?**
Hiányzó schema.org strukturált adatot ír egy termék metamezőjébe — olyan dolgokat, mint a meglévő termékopciókból levezetett műszaki specifikációk. Soha nem nyúl a termék címéhez, leírásához, képeihez vagy árához, és soha nem talál ki olyan adatot, amit nem tud ellenőrizni: egy hiányzó vonalkód például hiányzó marad, ahelyett hogy kitalálná.

**A FAQ-válaszok és az átírt leírások az AI kitalációi, vagy a valódi termékemen alapulnak?**
A modell csak azokat a termékadatokat látja, amelyek már megvannak nálad — cím, leírás, gyártó és műszaki specifikációk —, és kifejezett utasítást kap, hogy ne adjon hozzá semmit, ami nincs benne ezekben az adatokban. Minden FAQ-t vagy átírt leírást átnézel, mielőtt megjelenne; semmi nem kerül élesbe automatikusan.

**Mi történik az adataimmal, ha eltávolítom az alkalmazást?**
A bolt beállításai, a mentett auditok, a FAQ- és tartalomátírás-tervezetek, a visibility promptok és az AI-eredetű forgalom eseményei automatikusan törlődnek, amint a Shopify értesít minket az eltávolításról. Az alkalmazás semmit nem tart meg azután, hogy elhagyod.

**Lemondhatom vagy visszaválthatok anélkül, hogy kapcsolatba lépnék az ügyfélszolgálattal?**
Igen. Lépj az **Árazás** oldalra az alkalmazáson belül, és válts Free csomagra bármikor — ez azonnal életbe lép, e-mail nélkül.

## Csomaghatárok

| Funkció | Free | Grow | Unlimited |
|---|---|---|---|
| Katalógus audit | Első 20 termék, egyszeri, előzmények nélkül | Teljes katalógus + előzmények | Teljes katalógus + előzmények |
| Crawler szimulátor | 20/hónap | 300/hónap | 1000/hónap |
| Versenytárs-összehasonlítás | 10/hónap | 50/hónap | 150/hónap |
| FAQ generálás | Nem elérhető | 500/hónap | 500/hónap |
| Tartalom átírása | Nem elérhető | 300/hónap | 300/hónap |
| Visibility AI (követett promptok) | Nem elérhető | 5 prompt | 15 prompt |
| AI-eredetű forgalom pixel | Nem elérhető | Benne foglalt | Benne foglalt |
| AI ügyfélszolgálati chat | 1000 üzenet/hónap | 1000 üzenet/hónap | 1000 üzenet/hónap |
| Felület nyelvei | Mind a 30 | Mind a 30 | Mind a 30 |

Havi árazás: Free 0 $, Grow 9,99 $, Unlimited 19,99 $. Az éves fizetés Grow/Unlimited csomagon a havi fizetéshez képest nagyjából két hónapnyi kedvezményt jelent.

**Miért fedi le a Free csomag csak 20 terméket?**
Azért, hogy valódi eredményeket láthass a saját katalógusodon, mielőtt fizetős csomagra váltanál. A Grow és az Unlimited eltávolítja ezt a korlátot, és megőrzi a korábbi auditok teljes előzményét.

**Tényleg van korlát a FAQ generáláson még az Unlimited csomagon is?**
Igen — havi 500 generálás, szándékosan, még a legmagasabb csomagon is. Ez tartja fenntarthatóvá a funkciót a jelenlegi árszinten; ha nagy volumenű katalógusod van, és többre van szükséged, vedd fel velünk a kapcsolatot, és megoldjuk.

**Miért ugyanaz az AI ügyfélszolgálati chat minden csomagon?**
Ez tudatos termékdöntés, nem hiányosság: az ügyfélszolgálat mindenkinek jár, soha nem lesz fizetős megkülönböztető funkció. Az üzenetkorlát (1000/hónap) csak technikai védelemként létezik a visszaélések ellen, nem valós korlátként — egyetlen jogszerű felhasználás sem közelíti meg.

**Hibát találtam, vagy valami furcsának tűnik. Kinek szóljak?**
Írj a [info@ifgecommerce.com](mailto:info@ifgecommerce.com) címre azzal, amit láttál, és ha tudod, melyik termékről vagy oldalról van szó — ez általában elég ahhoz, hogy gyorsan a végére járjunk. Az alkalmazáson belüli AI ügyfélszolgálati chatet is használhatod, és kérheted, hogy emberrel beszélhess.

[← Vissza a Súgóközponthoz](index.html)
