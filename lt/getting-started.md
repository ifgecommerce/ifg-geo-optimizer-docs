---
title: IFG GEO Optimizer
description: „IFG GEO Optimizer“ Shopify programos dokumentacija, DUK ir teisiniai puslapiai.
lang: lt
---

# Darbo pradžia

<div class="lang-switcher">
{% include lang-switcher.html current="lt" slug="getting-started" %}
</div>

„IFG GEO Optimizer“ turi devynias sritis, pasiekiamas iš viršutinės navigacijos, kai tik nustatymas baigtas: **Dashboard**, **Audit catalog**, **Crawler AI**, **FAQ product**, **Link Coach**, **Visibility AI**, **Pricing**, **Settings** ir **Support**. Šis vadovas pereina per visas jas ta tvarka, kuria dažniausiai jomis naudojasi prekybininkai.

## 1. Įdiekite ir užbaikite nustatymo vedlį

Pirmą kartą atidarius programą, trumpas vedlys (apie 2 minutes) surenka pagrindinius dalykus: sąsajos kalbą, jūsų grąžinimo ir siuntimo politikos duomenis, įmonės informaciją, ir — vienintelį techniškai iš tikrųjų svarbų žingsnį — **GEO Schema** programos priedo (app embed) aktyvavimą temos redaktoriuje. Kol šis priedas neįjungtas, jokie vėlesni programos veiksmai nepasiekia jūsų parduotuvės vitrinos, tad šio žingsnio praleisti neverta. Bet kuriuo metu galite pakeisti bet kurį iš šių atsakymų skiltyje **Settings**.

## 2. Dashboard

Jūsų pagrindinis puslapis. Jame rodomas dabartinis GEO balas (iš paskutinio audito), **Readiness Matrix** su aštuoniais iš karto matomais signalais — turinio išgaunamumas, Organization schema, `llms.txt`, `agents.md`, prieiga crawler'iams, MCP paruoštumas, Link Coach ryšys ir AI nukreipiamas srautas — bei prioretizuotas „taisyk tai pirmiausia" sąrašas ir jūsų plano naudojimo skaitikliai (DUK generavimai, katalogo dydis). Viskas čia veda tiesiai į puslapį, kuriame galite tuo pasirūpinti.

## 3. Audit catalog

Spustelėkite **Rescan catalog**, kad patikrintumėte kiekvieną produktą pagal devynis struktūrizuotų duomenų laukus, kurių ieško paieškos varikliai: nuotrauka, aprašymas, prekės ženklas, SKU, GTIN, kaina, techninės specifikacijos, grąžinimo politika ir siuntimo politika. Produktai, kurių balas mažesnis nei 80/100, parodo tiksliai, ko trūksta.

- **Pataisymas vienu paspaudimu**: kai programa gali saugiai išvesti trūkstamus duomenis (dažniausiai technines specifikacijas iš jau esamų produkto parinkčių), matysite mygtuką **Fix**, kuris juos įrašo tiesiai į produkto struktūrizuotus duomenis. Laukams, kurių programa negali patikrinti, niekas nespėliojama — pavyzdžiui, trūkstamas brūkšninis kodas taip ir lieka trūkstamas, o ne sugalvojamas.
- **Turinio chunking balas**: kartu su struktūrizuotų duomenų patikra, kiekvienas produktas gauna atskirą išgaunamumo balą — ne „ar laukas yra", o „ar AI/RAG sistema iš tikrųjų gali išgauti aiškų faktą iš šio aprašymo". Menkas, prieveiksmiais perkrautas tekstas gauna žemesnį balą net ir su tobulu schema.org žymėjimu.
- **`llms.txt`**: sugeneruoja tikrą, standartus atitinkantį `llms.txt` failą, apibendrinantį jūsų katalogą AI sistemoms, patiekiamą tikrame parduotuvės šaknies adrese (`/llms.txt`), o ne paslėptą po app proxy keliu, kur crawler'iai jo nerastų.
- **`agents.md`**: sugeneruoja failą, apibūdinantį jūsų parduotuvę savarankiškiems apsipirkimo agentams — variantai, paieška, atsiskaitymas — sukurtą tik iš realių duomenų, kuriuos jūsų parduotuvė jau atskleidžia, nieko nesugalvojant.
- **Organization schema**: publikuoja jūsų įmonės duomenis (juridinis pavadinimas, PVM/mokesčių kodas, adresas) kaip struktūrizuotus duomenis, kad AI varikliai galėtų patikrinti, jog esate reali, atskaitinga įmonė, prieš jus rekomenduodami.

Free plane auditas apima pirmuosius 20 produktų, vienkartinis, be istorijos. Grow ir Unlimited planai nuskaito visą katalogą ir išsaugo kiekvieną praeitą nuskaitymą tendencijų palyginimui.

## 4. Crawler AI

Pasirinkite produktą, ir programa gauna jo puslapį lygiai taip, kaip tai daro AI crawler'is — be JavaScript vykdymo, kaip GPTBot, ClaudeBot ar PerplexityBot — taigi matote tiksliai tai, kas matoma šiems varikliams: ar jūsų `robots.txt` juos blokuoja (tikrinama kiekvienam botui atskirai, o ne tik bendru leidimu/draudimu), ir ar jūsų struktūrizuoti duomenys iš tikrųjų išlieka neapdorotame HTML, kurį šie botai skaito.

**Konkurentų palyginimas** (atskiras skirtukas šiame puslapyje): įklijuokite konkurento produkto URL ir gaukite tuos pačius GEO signalus, palygintus šalia jūsiškių — tokį patį skirtumą gautumėte iš rankinio audito, be poreikio registruotis konkurento pačiuose įrankiuose.

## 5. FAQ product

Grow arba Unlimited plane pasirinkite produktą ir spustelėkite **Generate FAQs**, kad gautumėte tris–penkias klausimų ir atsakymų poras, parengtas tik iš to produkto realaus pavadinimo, aprašymo, tiekėjo ir specifikacijų — modeliui aiškiai nurodyta niekada nepridėti detalės, kurios dar nėra jūsų duomenyse. Peržiūrėkite kiekvieną juodraštį; niekas nepublikuojama be jūsų aiškaus **Approve**. Patvirtintos DUK atsiranda gyvame produkto puslapyje ir yra pažymėtos kaip `FAQPage` struktūrizuoti duomenys, taigi jos yra ir žmonėms skaitomos, ir mašinoms cituojamos.

**Turinio perrašymas** (atskiras skirtukas šiame puslapyje): programa gali perrašyti produkto aprašymą taip, kad jame būtų daugiau patikrinamų faktų ir jį būtų lengviau cituoti generatyviam varikliui — visada matote palyginimą prieš/po ir patvirtinate prieš bet ką įrašant atgal į produktą.

## 6. Link Coach

Analizuoja, kaip gerai jūsų produktai tarpusavyje susiję per bendras kolekcijas, tiekėjus ir žymas — vidinis nuorodų teikimas yra signalas, kurį AI sistemos naudoja suprasti, ką apima visas jūsų katalogas, o ne tik vienas puslapis vienu metu. Rodo produktus be prasmingų ryšių ir paaiškinamus pasiūlymus, kaip tai ištaisyti.

## 7. Visibility AI

Pridėkite iki kelių užklausų, kurias realistiškai tikėtumėtės, kad klientas užduotų AI asistentui (limitas priklauso nuo jūsų plano — žr. Pricing žemiau), ir kiekvieną savaitę programa patikrina, ar Claude, ChatGPT, Gemini ir Perplexity mini jūsų parduotuvę atsakyme, stebint tai laikui bėgant kiekvienam varikliui atskirai. Grow ir Unlimited planuose taip pat rodoma, kaip lyginate su įvardytais konkurentais tomis pačiomis užklausomis.

**AI nukreipiamas srautas** (Grow ir Unlimited): lengvas, privatumą gerbiantis pikselis aptinka, kada apsilankymas parduotuvės vitrinoje iš tikrųjų kilo iš vieno iš šių AI variklių (per referrer, tik po to, kai lankytojas davė sutikimą analitikai per jūsų parduotuvės slapukų juostą), ir praneša, kiek tokių apsilankymų gavote per pastarąsias 7 dienas — tai antroji ciklo pusė, kurios pats matomumo stebėjimas negali parodyti: ne tik „ar esame minimi", bet ir „ar tas paminėjimas ką nors atsiuntė".

## 8. Support

Programoje (apačioje dešinėje esanti piktograma) veikia AI pokalbių asistentas, skirtas klausimams apie GEO, jūsų audito rezultatus ar tai, kaip veikia konkreti funkcija. Jei jis negali padėti, galite paprašyti pakalbėti su žmogumi, ir pokalbis persiunčiamas tiesiai IFG eCommerce.

## 9. Settings

Čia valdote nustatymo vedlio atsakymus (politikas, įmonės duomenis, sąsajos kalbą — perjunkite akimirksniu tarp 30 kalbų, be perkrovimo vėlavimo), pakartotinai patikrinate temos priedo aktyvavimą ir matote savo paskyros Shopify prieigos apimtis (scopes).

## 10. Pricing

**Pricing** rodo Free, Grow ir Unlimited planus greta, mėnesinį ar metinį apmokėjimą (metinis apmokėjimas abiejuose mokamuose planuose reiškia maždaug 2 mėnesius nemokamai). Galite bet kada atnaujinti, sumažinti planą arba grįžti prie Free tiesiai programoje — el. laiško rašyti nereikia. Žr. [DUK](faq.html) tikslius plano limitus.

Tai visas ciklas. Dauguma prekybininkų pakartotinai paleidžia auditą pridėję naujų produktų, patikrina crawler simuliatorių kaskart atnaujinę aprašymą, ir kas savaitę žvilgteli į Dashboard Readiness Matrix.

[← Atgal į Pagalbos centrą](index.html)
