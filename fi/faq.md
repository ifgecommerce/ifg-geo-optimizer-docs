---
title: IFG GEO Optimizer
description: Dokumentaatio, usein kysytyt kysymykset ja lakisivut Shopify-sovellukselle IFG GEO Optimizer.
lang: fi
---

# Usein kysytyt kysymykset

<div class="lang-switcher">
{% include lang-switcher.html current="fi" slug="faq" %}
</div>

**Mitä eroa on GEO:lla ja SEO:lla?**
Perinteinen SEO optimoi hakukoneille, jotka sijoittavat ja listaavat linkkejä. GEO (Generative Engine Optimization) optimoi tekoälyjärjestelmille, jotka lukevat sisältösi ja generoivat vastauksen tai suosituksen suoraan — ChatGPT, Perplexity, Gemini, Claude ja Google AI Overviews. Nämä kaksi menevät osittain päällekkäin, mutta GEO välittää asioista, joita klassiset SEO-työkalut eivät tarkista: onko tuotesivullasi täydellinen rakenteinen data, pystyykö tekoälycrawler todella lukemaan sisältösi suorittamatta JavaScriptiä, ja onko tekstisi kirjoitettu tavalla, joka on helppo siteerata ja lainata.

**Koskeeko sovellus koskaan asiakkaideni tietoja?**
Ei henkilökohtaisia asiakastietoja. Sovelluksen Shopify-käyttöoikeudet ovat `read_products`, `write_products`, `read_themes` ja `write_pixels` — katalogin lukeminen ja parantaminen, teemalaajennuksen aktiivisuuden tarkistaminen sekä anonyymin verkkokauppaliikenteen pikselin aktivointi (katso alla). Se ei koskaan pyydä tilauksia tai asiakastietoja. Katso [Tietosuojakäytäntö](privacy.html) täydellistä erittelyä varten.

**Mikä on tekoäly-ohjautuvan liikenteen pikseli, ja seuraako se asiakkaitani?**
Grow- ja Unlimited-paketeissa pieni Web Pixel havaitsee, kun verkkokauppakäynti saapuu tunnetulta tekoälymoottorilta (selaimen referrerin kautta), ja raportoi moottorin, sivun ja aikaleiman — ei mitään, mikä tunnistaisi kävijän, ei evästeitä, ei istuntotietoja. Se toimii vain, jos kävijä on jo antanut analytiikkasuostumuksen kauppasi evästebannerin kautta (Shopifyn Customer Privacy API). Sitä käytetään näyttämään Dashboard-ruutu ("Tekoäly-ohjautuva liikenne, viimeiset 7 päivää") — Visibility AI -seurannan vastinpari, joka kertoo, mainitaanko sinua, mutta ei sitä, lähettikö se maininta ketään.

**Mitä katalogin auditoinnin "Fix"-painike oikeastaan muuttaa?**
Se kirjoittaa puuttuvan schema.org-rakenteisen datan tuotteen metakenttään — asioita kuten teknisiä tietoja, jotka on johdettu olemassa olevista tuotevaihtoehdoistasi. Se ei koskaan koske tuotteesi otsikkoa, kuvausta, kuvia tai hintaa, eikä koskaan keksi dataa, jota se ei pysty vahvistamaan: puuttuva viivakoodi, esimerkiksi, pysyy puuttuvana sen sijaan, että se arvattaisiin.

**Ovatko FAQ-vastaukset ja uudelleenkirjoitetut kuvaukset tekoälyn keksimiä, vai perustuvatko ne oikeaan tuotteeseeni?**
Malli näkee vain sen tuotedatan, joka sinulla jo on — otsikon, kuvauksen, valmistajan ja tekniset tiedot — ja sitä on nimenomaisesti ohjeistettu olemaan lisäämättä mitään, mitä tuossa datassa ei ole. Tarkistat jokaisen FAQ:n tai uudelleenkirjoitetun kuvauksen ennen kuin se julkaistaan; mikään ei mene julki automaattisesti.

**Mitä tiedoilleni tapahtuu, jos poistan sovelluksen asennuksesta?**
Kauppasi asetukset, tallennetut auditoinnit, FAQ- ja sisällön uudelleenkirjoitusluonnokset, näkyvyyskehotteet ja tekoäly-ohjautuvan liikenteen tapahtumat poistetaan automaattisesti, kun Shopify ilmoittaa meille asennuksen poistosta. Sovellus ei säilytä mitään sen jälkeen, kun olet poistunut.

**Voinko peruuttaa tai alentaa pakettia ottamatta yhteyttä tukeen?**
Kyllä. Siirry **Pricing**-osioon sovelluksen sisällä ja vaihda Free-pakettiin milloin tahansa — se astuu voimaan välittömästi, sähköpostia ei tarvita.

## Pakettirajat

| Ominaisuus | Free | Grow | Unlimited |
|---|---|---|---|
| Katalogin auditointi | Ensimmäiset 20 tuotetta, kertaluonteinen, ei historiaa | Koko katalogi + historia | Koko katalogi + historia |
| Crawler-simulaattori | 20/kk | 300/kk | 1 000/kk |
| Kilpailijavertailu | 10/kk | 50/kk | 150/kk |
| FAQ-generointi | Ei sisälly | 500/kk | 500/kk |
| Sisällön uudelleenkirjoitus | Ei sisälly | 300/kk | 300/kk |
| Visibility AI (seuratut kehotteet) | Ei sisälly | 5 kehotetta | 15 kehotetta |
| Tekoäly-ohjautuvan liikenteen pikseli | Ei sisälly | Sisältyy | Sisältyy |
| Tekoälytukichat | 1 000 viestiä/kk | 1 000 viestiä/kk | 1 000 viestiä/kk |
| Käyttöliittymän kielet | Kaikki 30 | Kaikki 30 | Kaikki 30 |

Kuukausihinnat: Free $0, Grow $9.99, Unlimited $19.99. Vuosilaskutus Grow/Unlimited-paketeissa on suunnilleen kaksi kuukautta ilmaiseksi verrattuna kuukausittaiseen maksuun.

**Miksi Free-paketti kattaa vain 20 tuotetta?**
Tarkoituksena on antaa sinun nähdä todellisia tuloksia omasta katalogistasi ennen kuin sitoudut maksulliseen pakettiin. Grow ja Unlimited poistavat tämän rajan ja säilyttävät täydellisen historian aiemmista auditoinneista.

**Onko FAQ-generoinnissa todella katto myös Unlimited-paketissa?**
Kyllä — 500 generointia kuukaudessa, tarkoituksella, jopa ylimmässä paketissa. Tämä pitää ominaisuuden kestävänä nykyisellä hinnalla; jos sinulla on suurivolyyminen katalogi, joka tarvitsee enemmän, ota yhteyttä, niin löydämme ratkaisun.

**Miksi tekoälytukichat on sama kaikissa paketeissa?**
Kyse on tuotepäätöksestä, ei laiminlyönnistä: tuki sisältyy kaikille, ei koskaan maksullinen erottautumistekijä. Viestikatto (1 000/kk) on olemassa vain teknisenä suojana väärinkäyttöä vastaan, ei todellisena rajana — mikään laillinen käyttö ei tule lähellekään sitä.

**Löysin bugin tai jokin näyttää olevan väärin. Kenelle kerron siitä?**
Lähetä sähköpostia osoitteeseen [info@ifgecommerce.com](mailto:info@ifgecommerce.com) kertoen, mitä näit, ja jos mahdollista, mikä tuote tai sivu oli kyseessä — se riittää yleensä nopeaan jäljittämiseen. Voit myös käyttää sovelluksen sisäistä tekoälytukichattia ja pyytää puhua ihmisen kanssa.

[← Takaisin Ohjekeskukseen](index.html)
