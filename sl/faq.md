---
title: IFG GEO Optimizer
description: Dokumentacija, pogosta vprašanja in pravne strani za Shopify aplikacijo IFG GEO Optimizer.
lang: sl
---

# Pogosta vprašanja

<div class="lang-switcher">
{% include lang-switcher.html current="sl" slug="faq" %}
</div>

**Kakšna je razlika med GEO in SEO?**
Tradicionalni SEO optimizira za iskalnike, ki razvrščajo in naštevajo povezave. GEO (Generative Engine Optimization) optimizira za sisteme AI, ki berejo vašo vsebino in neposredno generirajo odgovor ali priporočilo — ChatGPT, Perplexity, Gemini, Claude in Google AI Overviews. Oba se prekrivata, vendar GEO upošteva stvari, ki jih klasična orodja SEO ne preverjajo: ali ima stran izdelka popolne strukturirane podatke, ali lahko pajek AI dejansko prebere vašo vsebino brez izvajanja JavaScripta, in ali je vaše besedilo napisano tako, da ga je enostavno citirati.

**Ali aplikacija kdaj dostopa do podatkov mojih strank?**
Ne, do osebnih podatkov strank ne dostopa. Dovoljenja aplikacije v Shopify so `read_products`, `write_products`, `read_themes` in `write_pixels` — branje in izboljševanje vašega kataloga, preverjanje, ali je vgrajeni element teme aktiven, ter aktivacija anonimnega piksela za promet spletne trgovine (glejte spodaj). Aplikacija nikoli ne zahteva naročil ali evidenc strank. Za popoln pregled glejte [Politiko zasebnosti](privacy.html).

**Kaj je piksel za napotitveni promet iz AI in ali sledi mojim strankam?**
Pri paketih Grow in Unlimited majhen Web Pixel zazna, ko obisk spletne trgovine prispe iz znanega sistema AI (prek referrerja brskalnika), in poroča sistem, stran ter časovni žig — nič, kar bi identificiralo obiskovalca, brez piškotkov, brez podatkov o seji. Deluje samo, če je obiskovalec že podal privolitev za analitiko prek pasice s piškotki vaše trgovine (Shopify Customer Privacy API). Uporablja se za prikaz ploščice na nadzorni plošči ("Napotitveni promet iz AI, zadnjih 7 dni") — dopolnilo k sledenju Vidnosti AI, ki pove, ali ste omenjeni, ne pa, ali je ta omemba komu poslala obiskovalce.

**Kaj gumb "Popravi" pri reviziji kataloga dejansko spremeni?**
Zapiše manjkajoče strukturirane podatke schema.org v metapolje izdelka — na primer tehnične specifikacije, izpeljane iz obstoječih možnosti izdelka. Nikoli se ne dotakne naslova, opisa, slik ali cene izdelka in nikoli ne izmisli podatkov, ki jih ne more preveriti: manjkajoča črtna koda, na primer, ostane manjkajoča, namesto da bi bila ugibana.

**Ali so odgovori na pogosta vprašanja in preoblikovani opisi izmišljeni s strani AI, ali temeljijo na mojem dejanskem izdelku?**
Model vidi samo podatke o izdelku, ki jih že imate — naslov, opis, dobavitelja in tehnične specifikacije — in ima izrecno navodilo, naj ne doda ničesar, česar v teh podatkih ni. Vsako pogosto vprašanje ali preoblikovan opis pregledate, preden se objavi; nič ne gre v živo samodejno.

**Kaj se zgodi z mojimi podatki, če odstranim aplikacijo?**
Konfiguracija vaše trgovine, shranjene revizije, osnutki pogostih vprašanj in preoblikovane vsebine, pozivi za vidnost ter dogodki napotitvenega prometa iz AI se samodejno izbrišejo, ko nas Shopify obvesti o odstranitvi. Aplikacija po vašem odhodu ne obdrži ničesar.

**Ali lahko prekličem ali znižam paket brez stika s podporo?**
Da. Pojdite v razdelek **Cenik** znotraj aplikacije in kadar koli preklopite na Free — sprememba začne veljati takoj, brez potrebe po e-pošti.

## Omejitve paketov

| Funkcija | Free | Grow | Unlimited |
|---|---|---|---|
| Revizija kataloga | Prvih 20 izdelkov, enkratno, brez zgodovine | Celoten katalog + zgodovina | Celoten katalog + zgodovina |
| Simulator pajkov | 20/mesec | 300/mesec | 1.000/mesec |
| Primerjava s konkurenco | 10/mesec | 50/mesec | 150/mesec |
| Generiranje pogostih vprašanj | Ni vključeno | 500/mesec | 500/mesec |
| Preoblikovanje vsebine | Ni vključeno | 300/mesec | 300/mesec |
| Vidnost AI (sledeni pozivi) | Ni vključeno | 5 pozivov | 15 pozivov |
| Piksel napotitvenega prometa iz AI | Ni vključeno | Vključeno | Vključeno |
| Klepet podpore AI | 1.000 sporočil/mesec | 1.000 sporočil/mesec | 1.000 sporočil/mesec |
| Jeziki vmesnika | Vseh 30 | Vseh 30 | Vseh 30 |

Mesečna cena: Free 0 $, Grow 9,99 $, Unlimited 19,99 $. Letno obračunavanje pri paketih Grow/Unlimited pomeni približno dva meseca brezplačno v primerjavi z mesečnim plačevanjem.

**Zakaj paket Free zajema samo 20 izdelkov?**
Namen je, da vidite resnične rezultate na svojem katalogu, preden se odločite za plačljiv paket. Grow in Unlimited odpravita to omejitev in ohranita popolno zgodovino preteklih revizij.

**Ali res obstaja omejitev generiranja pogostih vprašanj tudi pri paketu Unlimited?**
Da — 500 generiranj na mesec, namerno, tudi pri najvišjem paketu. To ohranja funkcijo trajnostno pri trenutni ceni; če imate katalog z velikim obsegom, ki potrebuje več, nas kontaktirajte in poiskali bomo rešitev.

**Zakaj je klepet podpore AI enak pri vsakem paketu?**
To je poslovna odločitev, ne spregled: pomoč je vključena za vse, nikoli kot plačljiva razlika. Omejitev sporočil (1.000/mesec) obstaja izključno kot tehnična zaščita pred zlorabo, ne kot realna omejitev — nobena legitimna uporaba se ji niti približa.

**Našel sem napako ali se mi zdi, da nekaj ni v redu. Komu naj sporočim?**
Pišite na [info@ifgecommerce.com](mailto:info@ifgecommerce.com) z opisom, kaj ste opazili, in če je mogoče, kateri izdelek ali stran — to običajno zadostuje za hitro rešitev. Uporabite lahko tudi klepet s podporo AI znotraj aplikacije in zaprosite za pogovor s človekom.

[← Nazaj v Center za pomoč](index.html)
