---
title: IFG GEO Optimizer
description: Dokumentation, FAQ og juridiske sider til Shopify-appen IFG GEO Optimizer.
lang: da
---

# Ofte stillede spørgsmål

<div class="lang-switcher">
{% include lang-switcher.html current="da" slug="faq" %}
</div>

**Hvad er forskellen på GEO og SEO?**
Traditionel SEO optimerer til søgemaskiner, der rangerer og lister links. GEO (Generative Engine Optimization) optimerer til AI-systemer, der læser dit indhold og genererer et svar eller en anbefaling direkte — ChatGPT, Perplexity, Gemini, Claude og Google AI Overviews. De to overlapper, men GEO tager sig af ting, klassiske SEO-værktøjer ikke tjekker: om din produktside har fuldstændige strukturerede data, om en AI-crawler faktisk kan læse dit indhold uden at udføre JavaScript, og om din tekst er skrevet på en måde, der er let at citere.

**Rører appen nogensinde ved mine kunders data?**
Nej, ingen personlige kundedata. Appens Shopify-tilladelser er `read_products`, `write_products`, `read_themes` og `write_pixels` — læsning og forbedring af dit katalog, kontrol af at temaembedden er aktiv, og aktivering af en anonym pixel til storefront-trafik (se nedenfor). Den anmoder aldrig om ordrer eller kundeoplysninger. Se [Privatlivspolitikken](privacy.html) for den fulde gennemgang.

**Hvad er AI-henvisningstrafik-pixlen, og sporer den mine kunder?**
På Grow og Unlimited registrerer en lille Web Pixel, når et besøg på storefronten kommer fra en kendt AI-motor (via browserens referrer), og rapporterer motoren, siden og et tidsstempel — intet, der identificerer den besøgende, ingen cookies, ingen sessiondata. Den kører kun, hvis den besøgende allerede har givet analysesamtykke gennem din butiks cookiebanner (Shopifys Customer Privacy API). Den bruges til at vise et Dashboard-felt ("AI-henvisningstrafik, seneste 7 dage") — modstykket til Visibility AI-sporingen, som fortæller dig, om du bliver nævnt, men ikke om den omtale sendte nogen.

**Hvad ændrer "Fix"-knappen i katalogauditten helt konkret?**
Den skriver manglende schema.org-strukturerede data til et produkt-metafelt — f.eks. tekniske specifikationer udledt af dine eksisterende produktvalgmuligheder. Den rører aldrig ved din produkttitel, beskrivelse, billeder eller pris, og den opfinder aldrig data, den ikke kan verificere: en manglende stregkode forbliver f.eks. manglende i stedet for at blive gættet.

**Er FAQ-svarene og de omskrevne beskrivelser opdigtet af AI, eller baseret på mit reelle produkt?**
Modellen ser kun de produktdata, du allerede har — titel, beskrivelse, leverandør og tekniske specifikationer — og er eksplicit instrueret i ikke at tilføje noget, der ikke findes i disse data. Du gennemgår hver FAQ eller omskrevet beskrivelse, før den publiceres; intet går live automatisk.

**Hvad sker der med mine data, hvis jeg afinstallerer appen?**
Din butikskonfiguration, gemte audits, FAQ- og content-rewrite-udkast, visibility-prompts og AI-henvisningstrafik-hændelser slettes automatisk, når Shopify giver os besked om afinstalleringen. Appen beholder intet, efter du er gået.

**Kan jeg annullere eller nedgradere uden at kontakte support?**
Ja. Gå til **Pricing** inde i appen og skift til Free når som helst — det træder i kraft med det samme, ingen e-mail nødvendig.

## Plangrænser

| Funktion | Free | Grow | Unlimited |
|---|---|---|---|
| Katalogaudit | Første 20 produkter, engangs, ingen historik | Fuldt katalog + historik | Fuldt katalog + historik |
| Crawler-simulator | 20/måned | 300/måned | 1.000/måned |
| Konkurrentsammenligning | 10/måned | 50/måned | 150/måned |
| FAQ-generering | Ikke inkluderet | 500/måned | 500/måned |
| Omskrivning af indhold | Ikke inkluderet | 300/måned | 300/måned |
| Visibility AI (sporede prompts) | Ikke inkluderet | 5 prompts | 15 prompts |
| AI-henvisningstrafik-pixel | Ikke inkluderet | Inkluderet | Inkluderet |
| AI-supportchat | 1.000 beskeder/måned | 1.000 beskeder/måned | 1.000 beskeder/måned |
| Grænsefladesprog | Alle 30 | Alle 30 | Alle 30 |

Månedlig pris: Free $0, Grow $9.99, Unlimited $19.99. Årlig fakturering på Grow/Unlimited giver cirka to måneder gratis sammenlignet med månedlig betaling.

**Hvorfor dækker Free-planen kun 20 produkter?**
Det er ment til at lade dig se reelle resultater på dit eget katalog, før du forpligter dig til en betalt plan. Grow og Unlimited fjerner det loft og gemmer en fuld historik over tidligere audits.

**Er der virkelig et loft på FAQ-generering, selv på Unlimited?**
Ja — 500 genereringer om måneden, bevidst, selv på den øverste plan. Dette holder funktionen bæredygtig til den nuværende pris; hvis du har et katalog med stort volumen, der har brug for mere, så kontakt os, og vi finder en løsning.

**Hvorfor er AI-supportchatten den samme på alle planer?**
Det er en produktbeslutning, ikke en forglemmelse: assistance er inkluderet for alle, aldrig et betalt differentieringspunkt. Beskedloftet (1.000/måned) findes udelukkende som en teknisk sikkerhedsforanstaltning mod misbrug, ikke som en reel begrænsning — ingen legitim brug kommer i nærheden af det.

**Jeg har fundet en fejl, eller noget ser forkert ud. Hvem fortæller jeg det til?**
Send en e-mail til [info@ifgecommerce.com](mailto:info@ifgecommerce.com) med hvad du så, og hvis muligt, hvilket produkt eller hvilken side — det er som regel nok til at spore det hurtigt. Du kan også bruge AI-supportchatten inde i appen og bede om at tale med et menneske.

[← Tilbage til Hjælpecenter](index.html)
