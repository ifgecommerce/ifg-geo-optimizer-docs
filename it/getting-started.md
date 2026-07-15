---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
lang: it
---

# Guida introduttiva

<div class="lang-switcher">
{% include lang-switcher.html current="it" slug="getting-started" %}
</div>

IFG GEO Optimizer ha nove aree, tutte raggiungibili dalla barra di navigazione una volta completata la configurazione iniziale: **Dashboard**, **Audit catalogo**, **Crawler AI**, **FAQ prodotto**, **Link Coach**, **Visibilità AI**, **Piani**, **Impostazioni** e **Assistenza**. Questa guida le percorre tutte, nell'ordine in cui la maggior parte dei negozianti le usa.

## 1. Installa e completa la configurazione guidata

Al primo avvio, una breve configurazione guidata (circa 2 minuti) raccoglie le basi: lingua dell'interfaccia, dettagli delle politiche di reso e spedizione, dati aziendali e — l'unico passaggio davvero determinante tecnicamente — l'attivazione del blocco **GEO Schema** nell'editor del tema. Nessuna delle azioni successive dell'app raggiunge il tuo negozio finché questo blocco non è attivo, quindi conviene non saltarlo. Puoi sempre modificare ogni risposta in seguito da **Impostazioni**.

## 2. Dashboard

La tua base operativa. Mostra il tuo punteggio GEO attuale (dall'ultimo audit), una **Matrice di prontezza** con otto segnali a colpo d'occhio — estraibilità del contenuto, schema Organization, `llms.txt`, `agents.md`, accesso crawler, prontezza MCP, connettività Link Coach e traffico da citazioni AI — più un elenco prioritario di cosa sistemare prima e i contatori d'uso del tuo piano (generazioni FAQ, dimensione catalogo). Tutto qui rimanda direttamente alla pagina dove puoi agire.

## 3. Audit catalogo

Clicca **Rianalizza catalogo** per controllare ogni prodotto contro nove campi di dati strutturati che i motori di ricerca cercano: immagine, descrizione, brand, SKU, GTIN, prezzo, specifiche tecniche, politica di reso e politica di spedizione. I prodotti sotto 80/100 mostrano esattamente cosa manca.

- **Fix one-click**: dove l'app può derivare in sicurezza il dato mancante (di solito specifiche tecniche dalle opzioni prodotto già esistenti), vedrai un bottone **Correggi** che lo scrive direttamente nei dati strutturati del prodotto. Nessun dato viene indovinato per i campi che l'app non può verificare — un codice a barre mancante, ad esempio, resta mancante invece di essere inventato.
- **Punteggio di chunking dei contenuti**: oltre al controllo dei dati strutturati, ogni prodotto riceve un punteggio di estraibilità separato — non "il campo c'è" ma "un sistema AI/RAG riesce davvero a estrarre un fatto pulito da questa descrizione." Un testo debole e ricco di aggettivi ottiene un punteggio basso anche con un markup schema.org perfetto.
- **`llms.txt`**: genera un vero file `llms.txt` conforme allo standard che riassume il tuo catalogo per i sistemi AI, servito sulla vera root del negozio (`/llms.txt`), non nascosto sotto un path proxy dove i crawler non lo troverebbero.
- **`agents.md`**: genera un file che descrive il tuo negozio agli agenti di acquisto autonomi — varianti, ricerca, checkout — costruito solo da dati reali già esposti dal negozio, nulla di inventato.
- **Schema Organization**: pubblica i dati della tua azienda (ragione sociale, P.IVA, indirizzo) come dati strutturati, così i motori AI possono verificare che sei un'azienda reale e affidabile prima di consigliarti.

Sul piano Free, gli audit coprono i primi 20 prodotti, una tantum, senza storico. Grow e Unlimited analizzano l'intero catalogo e conservano ogni scansione passata per il confronto nel tempo.

## 4. Crawler AI

Scegli un prodotto e l'app ne recupera la pagina esattamente come farebbe un crawler AI — senza esecuzione JavaScript, come GPTBot, ClaudeBot o PerplexityBot — così vedi con precisione cosa è visibile a questi motori: se il tuo `robots.txt` li blocca (controllato per singolo bot, non solo un permesso/blocco generico), e se i tuoi dati strutturati sopravvivono davvero nell'HTML grezzo che questi bot leggono.

**Confronto competitivo** (scheda separata da questa pagina): incolla l'URL di un prodotto competitor e ottieni gli stessi segnali GEO messi a confronto fianco a fianco con i tuoi — la stessa differenza che otterresti da un audit manuale, senza doverti iscrivere agli strumenti del competitor.

## 5. FAQ prodotto

Su Grow o Unlimited, scegli un prodotto e clicca **Genera FAQ** per tre-cinque coppie domanda-risposta scritte solo dal titolo, dalla descrizione, dal brand e dalle specifiche reali di quel prodotto — al modello è esplicitamente vietato aggiungere un dettaglio non già presente in quei dati. Rivedi ogni bozza; nulla si pubblica senza il tuo **Approva** esplicito. Le FAQ approvate appaiono sulla pagina prodotto live e sono marcate come dati strutturati `FAQPage`, quindi sono leggibili sia da una persona sia citabili da una macchina.

**Riscrittura contenuti** (scheda separata da questa pagina): l'app può riscrivere la descrizione di un prodotto per renderla più densa di fatti verificabili e più facile da citare per un motore generativo — vedi sempre un confronto prima/dopo e approvi prima che qualcosa venga scritto sul prodotto.

## 6. Link Coach

Analizza quanto i tuoi prodotti sono collegati tra loro tramite collezioni condivise, vendor e tag — il collegamento interno è un segnale che i sistemi AI usano per capire cosa copre il tuo catalogo nel suo insieme, non solo una pagina alla volta. Mostra i prodotti isolati senza collegamenti significativi e suggerimenti spiegabili per sistemarli.

## 7. Visibilità AI

Aggiungi fino a un numero limitato di domande che ti aspetteresti realisticamente da un cliente che chiede a un assistente AI (il limite dipende dal tuo piano — vedi Piani sotto), e ogni settimana l'app verifica se Claude, ChatGPT, Gemini e Perplexity citano il tuo negozio nella risposta, tracciato nel tempo per ogni motore. Su Grow e Unlimited, mostra anche come ti confronti con competitor nominati sulle stesse domande.

**Traffico da citazioni AI** (Grow e Unlimited): un pixel leggero e rispettoso della privacy rileva quando una visita al negozio arriva davvero da uno di questi motori AI (tramite il referrer, solo dopo che il visitatore ha dato il consenso all'analisi tramite il banner cookie del negozio) e riporta quante visite di questo tipo hai avuto negli ultimi 7 giorni — la seconda metà del quadro che il solo tracking visibilità non può mostrare: non solo "siamo citati," ma "quella citazione sta mandando qualcuno."

## 8. Assistenza

Un assistente chat AI vive nell'app (icona in basso a destra) per domande su GEO, sui risultati del tuo audit o su come funziona una specifica funzione. Se non riesce ad aiutarti, puoi chiedere di parlare con una persona e la conversazione viene inoltrata direttamente a IFG eCommerce.

## 9. Impostazioni

Dove gestisci le risposte della configurazione guidata (politiche, dati aziendali, lingua dell'interfaccia — cambio istantaneo tra 30 lingue, senza ricaricamenti lenti), riverifichi l'attivazione del blocco tema, e vedi gli scope Shopify del tuo account.

## 10. Piani

**Piani** mostra Free, Grow e Unlimited a confronto, mensile o annuale (l'annuale su entrambi i piani a pagamento equivale a circa 2 mesi gratis). Puoi passare a un piano superiore, tornare a uno inferiore, o cancellare tornando a Free in qualsiasi momento, direttamente dall'app — nessuna email richiesta. Vedi le [FAQ](faq.html) per i limiti esatti dei piani.

Questo è il ciclo completo. La maggior parte dei negozianti rilancia un audit dopo aver aggiunto nuovi prodotti, controlla il crawler simulator ogni volta che aggiorna una descrizione, e dà un'occhiata alla Matrice di prontezza della Dashboard con cadenza settimanale.

[← Torna al Centro Assistenza](index.html)
