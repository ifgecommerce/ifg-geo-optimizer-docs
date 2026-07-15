---
title: IFG GEO Optimizer
description: Dokumentazzjoni, Mistoqsijiet Frekwenti, u paġni legali għall-app Shopify IFG GEO Optimizer.
lang: mt
---

# L-Ewwel Passi

<div class="lang-switcher">
{% include lang-switcher.html current="mt" slug="getting-started" %}
</div>

IFG GEO Optimizer għandu disa' żoni, kollha aċċessibbli min-navigazzjoni ta' fuq ladarba l-konfigurazzjoni tispiċċa: **Dashboard**, **Audit tal-katalgu**, **Crawler AI**, **FAQ tal-prodott**, **Link Coach**, **Viżibbiltà AI**, **Prezzijiet**, **Settings**, u **Appoġġ**. Din il-gwida tgħaddi minn kollha, fl-ordni li fih il-biċċa l-kbira tan-negozjanti jużawhom.

## 1. Installa u lesta l-konfigurazzjoni gwidata

Mal-ewwel ftuħ, konfigurazzjoni gwidata qasira (madwar 2 minuti) tiġbor l-affarijiet bażiċi: il-lingwa tal-interfaċċja, id-dettalji tal-politika ta' ritorn u kunsinna tiegħek, l-informazzjoni dwar il-kumpanija tiegħek, u — l-uniku pass li verament jgħodd teknikament — l-attivazzjoni tal-app embed **GEO Schema** fl-editor tat-tema tiegħek. Xejn minn dak li tagħmel l-app wara ma jilħaqx il-ħanut tiegħek qabel ma dan l-embed jiġi attivat, għalhekk ħaqqu ma taqbżux. Tista' dejjem tibdel kwalunkwe waħda minn dawn it-tweġibiet aktar tard minn **Settings**.

## 2. Dashboard

Il-bażi tiegħek. Turi l-punteġġ GEO attwali tiegħek (mill-aħħar verifika), **Matriċi tal-Lestezza** b'tmien sinjali f'daqqa t'għajn — l-estraibbiltà tal-kontenut, l-iskema Organization, `llms.txt`, `agents.md`, l-aċċess tal-crawler, il-lestezza MCP, il-konnettività tal-Link Coach, u t-traffiku ta' referral mill-AI — flimkien ma' lista ta' prijorità "irranġa dan l-ewwel" u l-kontaturi tal-użu tal-pjan tiegħek (ġenerazzjonijiet ta' FAQ, daqs tal-katalgu). Kollox hawn jgħaqqdek direttament mal-paġna fejn tista' taġixxi fuqu.

## 3. Audit tal-katalgu

Ikklikkja **Skennja mill-ġdid il-katalgu** biex tivverifika kull prodott skont disa' oqsma ta' dejta strutturata li l-magni tat-tiftix ifittxu: ritratt, deskrizzjoni, marka, SKU, GTIN, prezz, speċifikazzjonijiet tekniċi, politika ta' ritorn, u politika ta' kunsinna. Il-prodotti taħt 80/100 juru eżattament x'jonqoshom.

- **Sewwi b'click wieħed**: fejn l-app tista' b'mod sikur toħroġ id-dejta nieqsa (ġeneralment speċifikazzjonijiet tekniċi mill-għażliet eżistenti tal-prodott), tara buttuna **Sewwi** li tiktibha direttament fid-dejta strutturata tal-prodott. Xejn ma jiġi ivvintat għall-oqsma li l-app ma tistax tivverifika — barcode nieqes, pereżempju, jibqa' nieqes minflok ma jiġi ivvintat.
- **Punteġġ ta' content chunking**: flimkien mal-verifika tad-dejta strutturata, kull prodott jirċievi punteġġ ta' estraibbiltà separat — mhux "il-qasam hemm" imma "sistema AI/RAG tista' verament tislet fatt nadif minn din id-deskrizzjoni." Test rqiq, mimli aġġettivi, jieħu punteġġ aktar baxx anke b'markup schema.org perfett.
- **`llms.txt`**: jiġġenera fajl `llms.txt` reali u konformi mal-istandard li jiġbor fil-qosor il-katalgu tiegħek għas-sistemi AI, servut fuq ir-root vera tal-ħanut tiegħek (`/llms.txt`), mhux moħbi taħt path ta' app proxy fejn il-crawlers ma jsibuhx.
- **`agents.md`**: jiġġenera fajl li jiddeskrivi l-ħanut tiegħek lill-aġenti awtonomi tax-xiri — varjanti, tfittxija, checkout — mibni biss minn dejta reali li l-ħanut tiegħek diġà juri, xejn ivvintat.
- **Skema Organization**: jippubblika d-dettalji tal-kumpanija tiegħek (isem legali, numru tal-VAT/taxxa, indirizz) bħala dejta strutturata, sabiex il-magni AI jkunu jistgħu jivverifikaw li int negozju reali u responsabbli qabel ma jirrakkomandawk.

Fuq Free, il-verifiki jkopru l-ewwel 20 prodott tiegħek, darba biss, mingħajr storja miżmuma. Grow u Unlimited jiskennjaw il-katalgu sħiħ tiegħek u jżommu kull skennjar tal-passat għal paragun tax-xejra.

## 4. Crawler AI

Agħżel prodott u l-app tiġbed il-paġna tiegħu eżattament bl-istess mod ta' crawler AI — mingħajr eżekuzzjoni ta' JavaScript, l-istess bħal GPTBot, ClaudeBot, jew PerplexityBot — sabiex tara preċiżament x'inhu viżibbli għal dawn il-magni: jekk `robots.txt` tiegħek jimblokkahomx (ivverifikat għal kull bot separatament, mhux biss permess/projbizzjoni ġenerika), u jekk id-dejta strutturata tiegħek verament tibqax fl-HTML mhux ipproċessat li dawn il-bots jaqraw.

**Paragun mal-kompetituri** (tab għaliha nnifisha minn din il-paġna): waħħal l-URL tal-prodott ta' kompetitur u ħu l-istess sinjali GEO mqabbla ħdejn xulxin mat-tiegħek — l-istess differenza li kieku tikseb minn verifika manwali, mingħajr ma jkollok bżonn tirreġistra fl-għodod tal-kompetitur stess.

## 5. FAQ tal-prodott

Fuq Grow jew Unlimited, agħżel prodott u ikklikkja **Iġġenera l-FAQs** għal tlieta sa ħames paretenzi ta' mistoqsija-u-tweġiba miktuba biss mit-titlu, id-deskrizzjoni, il-bejjiegħ, u l-ispeċifikazzjonijiet reali ta' dak il-prodott — il-mudell huwa mgħoddi struzzjoni espliċita li qatt ma jżid dettall li mhux diġà fid-dejta tiegħek. Irrevedi kull abbozz; xejn ma jiġi ppubblikat mingħajr **Approva** espliċitu tiegħek. Il-FAQs approvati jidhru fil-paġna tal-prodott ħajja u huma mmarkati bħala dejta strutturata `FAQPage`, għalhekk huma kemm jinqraw minn bniedem kif ukoll jistgħu jiġu ċċitati minn magna.

**Kitba mill-ġdid tal-kontenut** (tab għaliha nnifisha minn din il-paġna): l-app tista' terġa' tikteb id-deskrizzjoni ta' prodott biex tkun aktar densa fi fatti verifikabbli u eħfef biex magna ġenerattiva tikkwotaha — dejjem tara paragun ta' qabel/wara u tapprova qabel ma xi ħaġa tinkiteb lura fuq il-prodott.

## 6. Link Coach

Janalizza kemm il-prodotti tiegħek huma konnessi ma' xulxin permezz ta' kollezzjonijiet, bejjiegħa, u tikketti (tags) kondiviżi — il-konnessjoni interna hija sinjal li s-sistemi AI jużaw biex jifhmu x'jkopri l-katalgu tiegħek b'mod sħiħ, mhux biss paġna waħda kull darba. Juri l-prodotti orfni mingħajr konnessjonijiet siwjin u suġġerimenti spjegabbli biex issewwi dan.

## 7. Viżibbiltà AI

Żid sa ftit prompts li realistikament tistenna li klijent jistaqsi lil assistent AI (il-limitu jiddependi mill-pjan tiegħek — ara Prezzijiet hawn taħt), u kull ġimgħa l-app tivverifika jekk Claude, ChatGPT, Gemini, u Perplexity isemmux il-ħanut tiegħek fit-tweġiba, imsegwit maż-żmien għal kull magna. Fuq Grow u Unlimited, dan juri wkoll kif tqabbel ma' kompetituri msemmija fuq l-istess prompts.

**Traffiku ta' referral mill-AI** (Grow u Unlimited): pixel ħafif u rispettuż tal-privatezza jinnota meta żjara lill-ħanut verament toriġina minn waħda minn dawn il-magni AI (permezz tar-referrer, biss wara li ż-żaġġaġ ikun ta l-kunsens tal-analitika permezz tal-banner tal-cookies tal-ħanut tiegħek) u jirrapporta kemm żjarat bħal dawn kellek fl-aħħar 7 ijiem — it-tieni nofs taċ-ċiklu li t-traċċar tal-viżibbiltà waħdu ma jistax juri: mhux biss "aħna msemmija," imma "dik il-msemmija qed tibgħat lil xi ħadd."

## 8. Appoġġ

Assistent taċ-chat bl-AI jgħix ġewwa l-app (ikona fil-kantuniera t'isfel lemin) għal mistoqsijiet dwar GEO, ir-riżultati tal-verifika tiegħek, jew kif taħdem karatteristika speċifika. Jekk ma jkunx jista' jgħinek, tista' titlob titkellem ma' bniedem u l-konversazzjoni tintbagħat direttament lil IFG eCommerce.

## 9. Settings

Fejn timmaniġġja t-tweġibiet tal-konfigurazzjoni gwidata (politiki, dejta tal-kumpanija, lingwa tal-interfaċċja — biddel istantanjament bejn 30 lingwa, mingħajr dewmien ta' reload), tivverifika mill-ġdid l-attivazzjoni tal-embed tat-tema, u tara l-iskopijiet (scopes) ta' Shopify tal-kont tiegħek.

## 10. Prezzijiet

**Prezzijiet** juri Free, Grow, u Unlimited ħdejn xulxin, kull xahar jew kull sena (kull sena hija bejn wieħed u ieħor xahrejn b'xejn fuq iż-żewġ pjani mħallsa). Tista' tgħolli l-pjan, tniżżlu, jew tikkanċella lura għal Free fi kwalunkwe ħin, direttament mill-app — l-ebda email meħtieġa. Ara l-[Mistoqsijiet Frekwenti](faq.html) għal-limiti eżatti tal-pjan.

Dak huwa ċ-ċiklu sħiħ. Il-biċċa l-kbira tan-negozjanti jerġgħu jħaddmu verifika wara li jżidu prodotti ġodda, jiċċekkjaw is-simulatur tal-crawler kull darba li jaġġornaw deskrizzjoni, u jagħtu ħarsa lejn il-Matriċi tal-Lestezza tad-Dashboard kull ġimgħa.

[← Lura lejn iċ-Ċentru ta' Għajnuna](index.html)
