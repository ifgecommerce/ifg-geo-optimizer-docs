---
title: IFG GEO Optimizer
description: Dokumentáció, GYIK és jogi oldalak az IFG GEO Optimizer Shopify alkalmazáshoz.
lang: hu
---

# Adatvédelmi szabályzat

<div class="lang-switcher">
{% include lang-switcher.html current="hu" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify alkalmazás a Generative Engine Optimization számára
Utolsó frissítés: 2026. július

## 1. Adatkezelő

Az **IFG GEO Optimizer** alkalmazáson keresztül feldolgozott személyes adatok adatkezelője:

**IFG eCommerce** — székhely: Róma, Olaszország
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Milyen adatokat gyűjtünk

- **Kereskedői fiókadatok (Shopify OAuth-on keresztül)**: a bolt domainje, egy API hozzáférési token, valamint a Shopify fiókodhoz tartozó e-mail cím.
- **Katalógusadatok (csak olvasás)**: termékcímek, leírások, gyártó, árak, opciók és műszaki specifikációk — auditok futtatásához, a crawler-viselkedés szimulálásához, a tartalom kinyerhetőségének pontozásához, valamint FAQ-k vagy átírt leírások tervezetének elkészítéséhez használjuk.
- **Bolt beállításai**: az aktív csomagod, a Beállításokban megadott visszaküldési és szállítási szabályzat adatai és cégadatok, mentett auditok, FAQ- és tartalomátírás-tervezetek, valamint az AI-láthatóság követésére kiválasztott promptok.
- **Ügyfélszolgálati chat üzenetek**: a szöveg, amelyet az alkalmazáson belüli AI asszisztenssel váltasz, beleértve a hozzánk továbbított átiratot is, ha kifejezetten kéred, hogy emberrel beszélhess.
- **Anonim webáruház-forgalom (Web Pixel, Grow/Unlimited)**: amikor egy látogató egy felismert AI motorból (ChatGPT, Perplexity, Claude, Gemini, Copilot) érkezik egy termékoldalra, rögzítjük a motort, az oldal URL-jét és egy időbélyeget — csak akkor, ha a látogató már hozzájárult az analitikai adatgyűjtéshez a bolt cookie-bannerén keresztül. Nem gyűjtünk látogatóazonosítót, cookie-t vagy munkamenet-adatot.
- **Technikai adatok**: kérés-időbélyegek, belső rekordazonosítók és rendszernaplók.

> Az alkalmazás **soha nem kér és nem kap személyes végfelhasználói (ügyfél) adatot** — sem nevet, sem e-mail címet, sem címet, sem rendelést. A kért Shopify jogosultságok: `read_products`, `write_products` (katalógus és strukturált adat), `read_themes` (a téma embed aktív állapotának ellenőrzése) és `write_pixels` (a fent említett anonim forgalmi pixel aktiválása).

## 3. Miért dolgozzuk fel, és milyen jogalapon

Ezeket az adatokat azért dolgozzuk fel, hogy nyújtani tudjuk azt a szolgáltatást, amelyért az alkalmazást telepítetted — a GDPR 6. cikk (1) bekezdés b) pontja alapján, szerződés teljesítése céljából: a katalógusod generatív keresőmotorokon való láthatóságának elemzése és javítása, beleértve az AI-alapú FAQ-tervezést és a tartalomátírást, az alkalmazáson belüli ügyfélszolgálati chatet, a te által választott promptokon végzett heti AI-láthatóság követést, valamint az anonim AI-eredetű forgalom mérését — mindezek vagy a kereskedő által kezdeményezettek, vagy a forgalmi pixel esetében hozzájáruláshoz kötöttek a webáruházadban.

## 4. Hogyan gyűjtjük

A fiókadatokat egyszer, a Shopify OAuth folyamatán keresztül gyűjtjük, telepítéskor. A katalógusadatokat a Shopify Admin API-n keresztül olvassuk, csak akkor, amikor a vezérlőpultról egy műveletet indítasz. A forgalmi pixel a webáruházadban fut, és csak hozzájárulás után jelent eseményeket; a háttérben semmi más nem fut anélkül, hogy te kérnéd.

## 5. Kikkel osztjuk meg

- **Google Firebase / Cloud Firestore** — tárolja a beállításaidat, munkameneteidet és tervezeteidet. A Google LLC (USA) részt vesz az EU-USA Adatvédelmi Keretrendszerben (Data Privacy Framework). Az adatok az europe-west1 régióban (Belgium) tárolódnak.
- **Anthropic PBC (USA)** — biztosítja a Claude modellt, amelyet a FAQ-tervezéshez, a tartalomátíráshoz és az alkalmazáson belüli ügyfélszolgálati chathez használunk, kizárólag a te kifejezett műveleted alapján. Csak a megadott termékattribútumokat vagy chat-szöveget kapja meg — soha ügyféladatot.
- **OpenAI, Inc. (USA)** és **Perplexity AI, Inc. (USA)** — kizárólag a te által kifejezetten kiválasztott promptok heti AI-láthatóság követésére használjuk. Csak a követett prompt szövegét kapják meg — soha ügyféladatot.
- **Google LLC (USA)** — biztosítja a Gemini modellt, amelyet ugyanúgy használunk, mint a fenti OpenAI/Perplexity szolgáltatókat a láthatóság követésére (ez különbözik a Firebase/Firestore szerepétől, amely kizárólag tárolás).
- **Resend, Inc. (USA)** — értesítést küld nekünk, a bolt nevével és az ügyfélszolgálati chat átiratával, csak akkor, ha kifejezetten kéred, hogy emberrel beszélhess az ügyfélszolgálati chatben.
- **Shopify Inc.** — maga a platform, valamint az Admin API és a Web Pixel infrastruktúra forrása, amelyet az alkalmazás használ.

Nem adunk el adatot, és nem használjuk marketing vagy viselkedési profilalkotás céljára.

## 6. Meddig őrizzük meg

- **Munkamenet-tokenek**: a Shopify offline-token életciklusa kezeli, automatikusan megújulnak.
- **Beállítások, auditok, tervezetek és forgalmi események**: az alkalmazás telepítésének teljes ideje alatt megőrizzük. Az eltávolítás kiváltja a Shopify `shop/redact` webhookját, amely teljesen törli a bolt beállításait és munkameneteit.
- **Technikai naplók**: a Google Cloud szabványos naplómegőrzési szabályai szerint őrizzük.

## 7. A te jogaid

A GDPR 15–22. cikke alapján kérheted az adataidhoz való hozzáférést, a pontatlan adatok helyesbítését vagy törlését — a legegyszerűbb módja az alkalmazás eltávolítása —, vagy tiltakozhatsz az adatkezelés ellen. Panaszt is tehetsz a helyi adatvédelmi hatóságnál. Mivel az alkalmazás soha nem dolgoz fel személyes végfelhasználói (ügyfél) adatot, a `customers/data_request` és a `customers/redact` megfelelőségi webhookok azzal a megerősítéssel válaszolnak, hogy nincs mit exportálni vagy törölni.

## 8. Biztonság

Minden forgalom HTTPS/TLS 1.2+ protokollon keresztül zajlik. A Shopify hitelesítési tokenek soha nem kerülnek a böngészőhöz. Minden webhookot állandó idejű (constant-time) HMAC SHA-256 ellenőrzéssel hitelesítünk, mielőtt feldolgoznánk. Az adatbázis csak a backendről érhető el, a hosting platform saját szolgáltatásazonosítóján keresztül hitelesítve — a kódban nincsenek statikus hitelesítő adatok, és a közvetlen kliens-hozzáférést az adatbázis saját biztonsági szabályai tiltják. Az adatok titkosítva vannak, mind tárolás, mind továbbítás közben.

## 9. Módosítások

Ezt a szabályzatot időről időre frissíthetjük. A lényeges változásokat itt tüntetjük fel, a lap tetején lévő dátumot pedig naprakészen tartjuk.

---

**Kérdésed van az adataiddal kapcsolatban?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Vissza a Súgóközponthoz](index.html)
