---
title: IFG GEO Optimizer
description: Dokumentaatio, usein kysytyt kysymykset ja lakisivut Shopify-sovellukselle IFG GEO Optimizer.
lang: fi
---

# Tietosuojakäytäntö

<div class="lang-switcher">
{% include lang-switcher.html current="fi" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Shopify-sovellus generatiivisten hakukoneiden optimointiin (Generative Engine Optimization)
Viimeksi päivitetty: heinäkuu 2026

## 1. Rekisterinpitäjä

IFG GEO Optimizerin kautta käsiteltyjen henkilötietojen rekisterinpitäjä on:

**IFG eCommerce** — kotipaikka Rooma, Italia
Sähköposti: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Mitä keräämme

- **Kauppiaan tilitiedot (Shopify OAuthin kautta)**: kauppasi verkkotunnus, API-käyttöoikeustunnus ja Shopify-tilisi sähköpostiosoite.
- **Katalogidata (vain luku)**: tuotteiden otsikot, kuvaukset, valmistaja, hinnat, vaihtoehdot ja tekniset tiedot — käytetään auditointien suorittamiseen, crawler-käyttäytymisen simulointiin, sisällön poimittavuuden pisteyttämiseen sekä FAQ-luonnosten tai uudelleenkirjoitettujen kuvausten laatimiseen.
- **Kaupan asetukset**: aktiivinen pakettisi, Settings-osiossa syöttämäsi palautus- ja toimituskäytännön tiedot ja yritystiedot, tallennetut auditoinnit, FAQ- ja sisällön uudelleenkirjoitusluonnokset sekä kehotteet, jotka valitset seurattavaksi tekoälynäkyvyyttä varten.
- **Tukichatin viestit**: teksti, jota vaihdat sovelluksen sisäisen tekoälyavustajan kanssa, mukaan lukien meille välitetty keskustelun tallenne, jos nimenomaisesti pyydät puhua ihmisen kanssa.
- **Anonyymi verkkokauppaliikenne (Web Pixel, Grow/Unlimited)**: kun kävijä saapuu tuotesivulle tunnistetulta tekoälymoottorilta (ChatGPT, Perplexity, Claude, Gemini, Copilot), tallennamme moottorin, sivun URL-osoitteen ja aikaleiman — vain jos kävijä on jo antanut analytiikkasuostumuksen kauppasi evästebannerin kautta. Mitään kävijätunnistetta, evästettä tai istuntotietoa ei kerätä.
- **Tekniset tiedot**: pyyntöjen aikaleimat, sisäiset tietuetunnisteet ja järjestelmälokit.

> Sovellus **ei koskaan pyydä eikä vastaanota loppuasiakkaiden henkilötietoja** — ei nimiä, sähköposteja, osoitteita eikä tilauksia. Pyydetyt Shopify-käyttöoikeudet ovat `read_products`, `write_products` (katalogi ja rakenteinen data), `read_themes` (teemalaajennuksen aktiivisuuden tarkistus) ja `write_pixels` (yllä kuvatun anonyymin liikennepikselin aktivointi).

## 3. Miksi käsittelemme tietoja, ja millä oikeusperusteella

Käsittelemme näitä tietoja tarjotaksemme palvelun, jota varten asensit sovelluksen — GDPR:n artiklan 6(1)(b) mukaisesti, sopimuksen täytäntöönpano: katalogisi näkyvyyden analysointi ja parantaminen generatiivisilla hakukoneilla, mukaan lukien tekoälyavusteinen FAQ-laadinta ja sisällön uudelleenkirjoitus, sovelluksen sisäinen tukichatti, viikoittainen tekoälynäkyvyyden seuranta valitsemillasi kehotteilla, ja anonyymi tekoäly-ohjautuvan liikenteen mittaus — kaikki joko kauppiaan itsensä käynnistämää tai, liikennepikselin osalta, kauppasi verkkokaupassa annettuun suostumukseen sidottua.

## 4. Miten keräämme tietoja

Tilitiedot kerätään kerran, Shopifyn OAuth-prosessin kautta, asennuksen yhteydessä. Katalogidata luetaan Shopifyn Admin API:n kautta vain, kun käynnistät toiminnon dashboardilta. Liikennepikseli toimii verkkokaupassasi ja raportoi tapahtumia vain suostumuksen jälkeen; mikään muu ei toimi taustalla ilman, että pyydät sitä.

## 5. Kenen kanssa jaamme tietoja

- **Google Firebase / Cloud Firestore** — tallentaa asetuksesi, istunnot ja luonnokset. Google LLC (USA) osallistuu EU-USA-tietosuojakehykseen (Data Privacy Framework). Data tallennetaan europe-west1-alueella (Belgia).
- **Anthropic PBC (USA)** — tarjoaa Claude-mallin, jota käytetään FAQ-laadintaan, sisällön uudelleenkirjoitukseen ja sovelluksen sisäiseen tukichattiin, vain nimenomaisen toimintasi perusteella. Vastaanottaa vain antamasi tuoteattribuutit tai chat-tekstin — ei koskaan asiakastietoja.
- **OpenAI, Inc. (USA)** ja **Perplexity AI, Inc. (USA)** — käytetään yksinomaan viikoittaiseen tekoälynäkyvyyden seurantaan kehotteilla, jotka nimenomaisesti valitset seurattavaksi. Vastaanottavat vain seuratun kehotteen tekstin — ei koskaan asiakastietoja.
- **Google LLC (USA)** — tarjoaa Gemini-mallin, jota käytetään samalla tavalla kuin OpenAI/Perplexity yllä näkyvyyden seurantaan (erillinen käyttötarkoitus verrattuna Firebase/Firestoreen, joka on vain tallennusta varten).
- **Resend, Inc. (USA)** — lähettää meille ilmoituksen, joka sisältää kaupan nimen ja tukichatin tallenteen, vain kun nimenomaisesti pyydät puhua ihmisen kanssa tukichatissa.
- **Shopify Inc.** — itse alusta, ja sovelluksen käyttämän Admin API:n ja Web Pixel -infrastruktuurin lähde.

Emme myy tietoja emmekä käytä niitä markkinointiin tai käyttäytymisprofiiliin.

## 6. Kuinka kauan säilytämme tietoja

- **Istuntotunnukset**: hallinnoidaan Shopifyn offline-tunnusten elinkaaren mukaisesti, uusitaan automaattisesti.
- **Asetukset, auditoinnit, luonnokset ja liikennetapahtumat**: säilytetään niin kauan kuin sovellus on asennettuna. Asennuksen poistaminen käynnistää Shopifyn `shop/redact`-webhookin, joka poistaa kauppasi asetukset ja istunnot kokonaan.
- **Tekniset lokit**: säilytetään Google Cloudin vakiolokien säilytyskäytännön mukaisesti.

## 7. Oikeutesi

GDPR:n artiklojen 15–22 mukaisesti voit pyytää pääsyä tietoihisi, virheellisten tietojen korjaamista tai poistamista — yksinkertaisin tapa on poistaa sovelluksen asennus — tai vastustaa käsittelyä. Voit myös tehdä valituksen paikalliselle tietosuojaviranomaisellesi. Koska sovellus ei koskaan käsittele loppuasiakkaiden henkilötietoja, `customers/data_request`- ja `customers/redact`-vaatimustenmukaisuuswebhookit vastaavat vahvistaen, ettei vietävää tai poistettavaa ole.

## 8. Tietoturva

Kaikki liikenne kulkee HTTPS/TLS 1.2+ -yhteyden kautta. Shopify-todennustunnuksia ei koskaan paljasteta selaimelle. Jokainen webhook varmennetaan vakioaikaisella HMAC SHA-256 -tarkistuksella ennen käsittelyä. Tietokanta on tavoitettavissa vain taustajärjestelmästä, todennettuna isännöintialustan omalla palveluidentiteetillä — koodissa ei ole staattisia tunnuksia, ja suora asiakaspääsy on estetty tietokannan omilla suojaussäännöillä. Data on salattu sekä levossa että siirron aikana.

## 9. Muutokset

Saatamme päivittää tätä käytäntöä aika ajoin. Olennaiset muutokset näkyvät täällä, ja yläreunan päivämäärä pidetään ajan tasalla.

---

**Kysymyksiä tiedoistasi?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Takaisin Ohjekeskukseen](index.html)
