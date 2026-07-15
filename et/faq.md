---
title: IFG GEO Optimizer
description: Shopify rakenduse IFG GEO Optimizer dokumentatsioon, KKK ja õiguslikud leheküljed.
lang: et
---

# Korduma Kippuvad Küsimused

<div class="lang-switcher">
{% include lang-switcher.html current="et" slug="faq" %}
</div>

**Mis vahe on GEO-l ja SEO-l?**
Traditsiooniline SEO optimeerib otsingumootoreid, mis pingerida ja loetlevad linke. GEO (Generative Engine Optimization) optimeerib AI süsteeme, mis loevad sinu sisu ja genereerivad vastuse või soovituse otse — ChatGPT, Perplexity, Gemini, Claude ja Google AI Overviews. Need kaks kattuvad, kuid GEO hoolib asjadest, mida klassikalised SEO tööriistad ei kontrolli: kas sinu tootelehel on täielikud struktureeritud andmed, kas AI crawler suudab tegelikult sinu sisu lugeda ilma JavaScripti käivitamata, ja kas sinu tekst on kirjutatud viisil, mida on lihtne tsiteerida ja viidata.

**Kas rakendus puudutab kunagi minu klientide andmeid?**
Ei, mitte mingeid isikuandmeid klientide kohta. Rakenduse Shopify õigused on `read_products`, `write_products`, `read_themes` ja `write_pixels` — sinu kataloogi lugemine ja parandamine, teema manuse aktiivsuse kontrollimine ning anonüümse poe liikluse piksli aktiveerimine (vaata allpool). See ei küsi kunagi tellimusi ega kliendiandmeid. Vaata täielikku ülevaadet [Privaatsuspoliitikast](privacy.html).

**Mis on AI-suunatud liikluse piksel ja kas see jälgib minu kliente?**
Grow ja Unlimited paketis tuvastab väike Web Pixel, kui poe külastus saabub teadaolevast AI mootorist (brauseri viitaja kaudu) ja raporteerib mootori, lehe ja ajatempli — mitte midagi, mis identifitseeriks külastajat, ei küpsiseid, ei seansiandmeid. See töötab ainult siis, kui külastaja on juba andnud analüütika nõusoleku sinu poe küpsisebänneri kaudu (Shopify Customer Privacy API). Seda kasutatakse Dashboardi kaardi ("AI-suunatud liiklus, viimased 7 päeva") näitamiseks — Visibility AI jälgimise vastandpool, mis ütleb, kas sind mainitakse, kuid mitte seda, kas see mainimine kellegi sinuni saatis.

**Mida "Fix" nupp kataloogi auditil tegelikult muudab?**
See kirjutab puuduvad schema.org struktureeritud andmed toote metaväljale — asjad nagu tehnilised andmed, mis on tuletatud sinu olemasolevatest tootevalikutest. See ei puuduta kunagi sinu toote pealkirja, kirjeldust, pilte ega hinda ning ei mõtle kunagi välja andmeid, mida ei saa kontrollida: näiteks puuduv triipkood jääb puuduvaks, selle asemel et seda ära arvata.

**Kas KKK vastused ja ümberkirjutatud kirjeldused on AI väljamõeldud või põhinevad minu tegelikul tootel?**
Mudel näeb ainult toote andmeid, mis sul juba on — pealkiri, kirjeldus, tootja ja tehnilised andmed — ning talle on selgesõnaliselt öeldud, et ei tohi lisada midagi, mida neis andmetes ei ole. Sa vaatad iga KKK või ümberkirjutatud kirjelduse üle enne selle avaldamist; miski ei lähe automaatselt avalikuks.

**Mis juhtub minu andmetega, kui ma rakenduse desinstallin?**
Sinu poe seadistus, salvestatud auditid, KKK ja sisu ümberkirjutamise mustandid, nähtavuse päringud ja AI-suunatud liikluse sündmused kustutatakse automaatselt, kui Shopify teavitab meid desinstallimisest. Rakendus ei säilita midagi pärast sinu lahkumist.

**Kas ma saan tühistada või alandada ilma toega ühendust võtmata?**
Jah. Mine rakenduses **Pricing** alla ja lülitu igal ajal Free peale — see rakendub koheselt, ilma e-kirjata.

## Paketilimiidid

| Funktsioon | Free | Grow | Unlimited |
|---|---|---|---|
| Kataloogi audit | Esimesed 20 toodet, ühekordselt, ilma ajaloota | Kogu kataloog + ajalugu | Kogu kataloog + ajalugu |
| Crawleri simulaator | 20/kuus | 300/kuus | 1,000/kuus |
| Konkurendi võrdlus | 10/kuus | 50/kuus | 150/kuus |
| KKK genereerimine | Ei sisaldu | 500/kuus | 500/kuus |
| Sisu ümberkirjutamine | Ei sisaldu | 300/kuus | 300/kuus |
| Visibility AI (jälgitavad päringud) | Ei sisaldu | 5 päringut | 15 päringut |
| AI-suunatud liikluse piksel | Ei sisaldu | Sisaldub | Sisaldub |
| AI tugivestlus | 1,000 sõnumit/kuus | 1,000 sõnumit/kuus | 1,000 sõnumit/kuus |
| Liidese keeled | Kõik 30 | Kõik 30 | Kõik 30 |

Kuutasu: Free $0, Grow $9.99, Unlimited $19.99. Aastane arveldus Grow/Unlimited paketil on ligikaudu kaks kuud tasuta võrreldes kuumaksega.

**Miks katab Free pakett ainult 20 toodet?**
Selle mõte on lasta sul näha päris tulemusi oma kataloogil enne tasulisele paketile üleminekut. Grow ja Unlimited eemaldavad selle piirangu ning säilitavad kõigi varasemate auditite täieliku ajaloo.

**Kas KKK genereerimisel on tõesti piirang isegi Unlimited paketil?**
Jah — 500 genereerimist kuus, teadlikult, isegi kõige kallimal paketil. See hoiab funktsiooni praeguse hinna juures jätkusuutlikuna; kui sul on suuremahuline kataloog, mis vajab rohkem, võta ühendust ja leiame lahenduse.

**Miks on AI tugivestlus igal paketil sama?**
See on tooteotsus, mitte tähelepanematus: abi on kõigile kaasas, mitte kunagi tasuline eristaja. Sõnumipiirang (1,000/kuus) on ainult tehniline kaitse kuritarvituse vastu, mitte reaalne piirang — ükski legitiimne kasutus ei jõua sellele isegi lähedale.

**Leidsin vea või midagi tundub vale olevat. Kellele ma sellest teatan?**
Kirjuta [info@ifgecommerce.com](mailto:info@ifgecommerce.com) ja kirjelda, mida nägid, ning võimalusel, millist toodet või lehte see puudutas — tavaliselt sellest piisab, et asi kiiresti üles leida. Samuti saad kasutada rakendusesisest AI tugivestlust ja küsida inimesega rääkimist.

[← Tagasi Abikeskusesse](index.html)
