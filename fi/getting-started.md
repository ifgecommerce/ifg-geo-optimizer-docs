---
title: IFG GEO Optimizer
description: Dokumentaatio, usein kysytyt kysymykset ja lakisivut Shopify-sovellukselle IFG GEO Optimizer.
lang: fi
---

# Aloitusopas

<div class="lang-switcher">
{% include lang-switcher.html current="fi" slug="getting-started" %}
</div>

IFG GEO Optimizerissa on yhdeksän osiota, jotka kaikki löytyvät yläpalkin navigaatiosta, kun asennus on valmis: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** ja **Support**. Tämä opas käy läpi ne kaikki siinä järjestyksessä, jossa useimmat kauppiaat niitä käyttävät.

## 1. Asenna ja suorita ohjattu käyttöönotto

Kun avaat sovelluksen ensimmäistä kertaa, lyhyt ohjattu käyttöönotto (noin 2 minuuttia) kerää perustiedot: käyttöliittymän kielen, palautus- ja toimituskäytäntösi tiedot, yrityksesi tiedot — sekä sen ainoan vaiheen, jolla on teknisesti todella merkitystä: **GEO Schema** -sovelluslaajennuksen aktivoinnin teemaeditorissa. Mikään, mitä sovellus tekee tämän jälkeen, ei tavoita verkkokauppaasi ennen kuin tämä laajennus on aktivoitu, joten sitä kannattaa olla ohittamatta. Voit aina muuttaa mitä tahansa näistä vastauksista myöhemmin **Settings**-osiosta.

## 2. Dashboard

Kotipesäsi. Se näyttää nykyisen GEO-pisteytyksesi (viimeisimmästä auditoinnista), **Readiness Matrix** -taulukon kahdeksalla silmäyksellä havaittavalla signaalilla — sisällön poimittavuus, Organization-schema, `llms.txt`, `agents.md`, crawler-pääsy, MCP-valmius, Link Coach -yhteydet ja tekoäly-ohjautuva liikenne — sekä priorisoidun "korjaa tämä ensin" -listan ja pakettisi käyttölaskurit (FAQ-generoinnit, katalogin koko). Kaikki tällä sivulla linkittyy suoraan sivulle, jossa voit toimia asian suhteen.

## 3. Audit catalog

Klikkaa **Rescan catalog** tarkistaaksesi jokaisen tuotteen yhdeksää rakenteisen datan kenttää vastaan, joita hakukoneet etsivät: kuva, kuvaus, brändi, SKU, GTIN, hinta, tekniset tiedot, palautuskäytäntö ja toimituskäytäntö. Alle 80/100 pisteen tuotteet näyttävät tarkalleen, mikä puuttuu.

- **Yhden klikkauksen korjaus**: kun sovellus voi turvallisesti johtaa puuttuvan tiedon (yleensä tekniset tiedot olemassa olevista tuotevaihtoehdoista), näet **Fix**-painikkeen, joka kirjoittaa sen suoraan tuotteen rakenteiseen dataan. Mitään ei arvata kenttien osalta, joita sovellus ei pysty vahvistamaan — puuttuva viivakoodi esimerkiksi pysyy puuttuvana sen sijaan, että se keksittäisiin.
- **Sisällön chunking-pisteytys**: rakenteisen datan tarkistuksen rinnalla jokainen tuote saa erillisen poimittavuuspisteen — ei sitä, "onko kenttä läsnä", vaan sitä, "pystyykö tekoäly-/RAG-järjestelmä oikeasti poimimaan siistin faktan tästä kuvauksesta". Ohut, adjektiivipainotteinen teksti saa alhaisemman pisteen, vaikka schema.org-merkintä olisi täydellinen.
- **`llms.txt`**: generoi todellisen, standardinmukaisen `llms.txt`-tiedoston, joka tiivistää kataloginne tekoälyjärjestelmille, ja joka tarjoillaan kauppanne todellisesta juuresta (`/llms.txt`), ei haudattuna sovellusproxy-polun alle, josta crawlerit eivät sitä löydä.
- **`agents.md`**: generoi tiedoston, joka kuvaa kauppaasi autonomisille ostosagenteille — variantit, haku, kassa — rakennettu vain todellisesta datasta, jonka kauppasi jo paljastaa, ei mitään keksittyä.
- **Organization-schema**: julkaisee yrityksesi tiedot (virallinen nimi, ALV-/verotunnus, osoite) rakenteisena datana, jotta tekoälymoottorit voivat vahvistaa, että olet todellinen, vastuullinen yritys ennen suosittelemistaan.

Free-paketissa auditoinnit kattavat ensimmäiset 20 tuotettasi, kertaluonteisesti, ilman historiaa. Grow ja Unlimited skannaavat koko katalogisi ja säilyttävät jokaisen aiemman skannauksen trendivertailua varten.

## 4. Crawler AI

Valitse tuote, ja sovellus hakee sen sivun täsmälleen samalla tavalla kuin tekoälycrawler tekisi — ilman JavaScriptin suoritusta, samoin kuin GPTBot, ClaudeBot tai PerplexityBot — jotta näet tarkalleen, mikä näkyy näille moottoreille: estääkö `robots.txt`-tiedostosi niitä (tarkistetaan botkohtaisesti, ei vain yleisellä salli/estä-säännöllä), ja säilyykö rakenteinen datasi todella raa'assa HTML:ssä, jota nämä botit lukevat.

**Kilpailijavertailu** (oma välilehtensä tällä sivulla): liitä kilpailijan tuote-URL ja saat samat GEO-signaalit rinnakkain vertailtuna omiisi — sama laadullinen ero, jonka saisit manuaalisesta auditoinnista, ilman että sinun tarvitsee rekisteröityä kilpailijan omiin työkaluihin.

## 5. FAQ product

Grow- tai Unlimited-paketissa valitse tuote ja klikkaa **Generate FAQs** saadaksesi kolmesta viiteen kysymys-vastaus-paria, jotka on laadittu vain kyseisen tuotteen todellisesta otsikosta, kuvauksesta, valmistajasta ja teknisistä tiedoista — mallille on nimenomaisesti ohjeistettu, ettei se koskaan lisää tietoa, joka ei jo ole datassasi. Tarkista jokainen luonnos; mikään ei julkaistu ilman nimenomaista **Approve**-hyväksyntääsi. Hyväksytyt FAQ:t näkyvät julkaistulla tuotesivulla ja on merkitty `FAQPage`-rakenteisena datana, joten ne ovat sekä ihmisen luettavissa että koneen siteerattavissa.

**Sisällön uudelleenkirjoitus** (oma välilehtensä tällä sivulla): sovellus voi kirjoittaa tuotekuvauksen uudelleen tiheämmäksi todennettavista faktoista ja helpommaksi generatiiviselle moottorille siteerata — näet aina ennen/jälkeen-vertailun ja hyväksyt ennen kuin mitään kirjoitetaan takaisin tuotteeseen.

## 6. Link Coach

Analysoi, kuinka hyvin tuotteesi ovat yhteydessä toisiinsa jaettujen kokoelmien, valmistajien ja tunnisteiden kautta — sisäinen linkitys on signaali, jota tekoälyjärjestelmät käyttävät ymmärtääkseen, mitä katalogisi kattaa kokonaisuutena, ei vain yhtä sivua kerrallaan. Näyttää orpotuotteet, joilla ei ole merkityksellisiä yhteyksiä, sekä selitetyt ehdotukset tilanteen korjaamiseksi.

## 7. Visibility AI

Lisää muutamia kehotteita, joita realistisesti odottaisit asiakkaan kysyvän tekoälyavustajalta (raja riippuu paketistasi — katso Pricing alla), ja joka viikko sovellus tarkistaa, mainitsevatko Claude, ChatGPT, Gemini ja Perplexity kauppaasi vastauksessa, seurattuna ajan mittaan moottorikohtaisesti. Grow- ja Unlimited-paketeissa tämä näyttää myös, miten vertaudut nimettyihin kilpailijoihin samoilla kehotteilla.

**Tekoäly-ohjautuva liikenne** (Grow ja Unlimited): kevyt, yksityisyyttä kunnioittava pikseli havaitsee, kun verkkokauppakäynti todella tulee yhdeltä näistä tekoälymoottoreista (referrerin kautta, vain sen jälkeen kun kävijä on antanut analytiikkasuostumuksen kauppasi evästebannerin kautta), ja raportoi, kuinka monta tällaista käyntiä sait viimeisen 7 päivän aikana — toinen puolisko silmukasta, jota pelkkä näkyvyyden seuranta ei voi näyttää: ei vain "mainitaanko meitä", vaan "lähettääkö se maininta ketään".

## 8. Support

Sovelluksessa on tekoälychat-avustaja (oikeassa alakulmassa oleva kuvake) kysymyksiin GEO:sta, auditointituloksistasi tai siitä, miten tietty ominaisuus toimii. Jos se ei pysty auttamaan, voit pyytää puhua ihmisen kanssa, ja keskustelu välitetään suoraan IFG eCommercelle.

## 9. Settings

Täällä hallinnoit ohjatun käyttöönoton vastauksia (käytännöt, yritystiedot, käyttöliittymän kieli — vaihda välittömästi 30 kielen välillä, ilman uudelleenlatausviivettä), tarkistat teemalaajennuksen aktivoinnin uudelleen ja näet tilisi Shopify-käyttöoikeudet.

## 10. Pricing

**Pricing** näyttää Free-, Grow- ja Unlimited-paketit rinnakkain, kuukausittain tai vuosittain (vuosilaskutus on suunnilleen 2 kuukautta ilmaiseksi molemmissa maksullisissa paketeissa). Voit päivittää, alentaa tai peruuttaa takaisin Free-pakettiin milloin tahansa, suoraan sovelluksesta — sähköpostia ei tarvita. Katso [Usein kysytyt kysymykset](faq.html) tarkkoja pakettirajoja varten.

Tämä on koko silmukka. Useimmat kauppiaat ajavat auditoinnin uudelleen uusien tuotteiden lisäämisen jälkeen, tarkistavat crawler-simulaattorin aina kun päivittävät kuvausta, ja vilkaisevat Dashboardin Readiness Matrixia viikoittain.

[← Takaisin Ohjekeskukseen](index.html)
