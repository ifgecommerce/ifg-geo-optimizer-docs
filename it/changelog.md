---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
lang: it
---

# Changelog

<div class="lang-switcher">
{% include lang-switcher.html current="it" slug="changelog" pages="en,it,de,fr,es" %}
</div>

Tutte le modifiche che raggiungono i negozianti, dalla più recente. Questa è documentazione tecnica, mantenuta in 5 lingue (italiano, inglese, tedesco, francese, spagnolo) invece delle 30 supportate dal resto del Centro Assistenza.

## Luglio 2026

**Tracking traffico da citazioni AI** — Aggiunto un Web Pixel (Grow/Unlimited) che rileva le visite allo storefront provenienti da un motore AI riconosciuto (ChatGPT, Perplexity, Claude, Gemini, Copilot) e le riporta su un nuovo tile della Dashboard, subordinato al consenso e completamente anonimo — il complemento del tracking Visibilità AI: non solo "siamo citati," ma "quella citazione sta mandando qualcuno."

**Rifinitura Dashboard e navigazione** — Aggiunto uno stato vuoto corretto per il primo utilizzo, uno skeleton di caricamento durante la navigazione tra pagine, e un dettaglio per singolo bot nella pagina crawler che mostra se una regola robots.txt è stata trovata per nome o ereditata dal gruppo wildcard.

**Nuova configurazione guidata** — La barra di progresso della configurazione guidata è diventata una checklist passo-passo, con un banner di conferma visibile al completamento invece di un ricaricamento istantaneo e non confermato.

**Fatturazione ed email di assistenza** — Il contatto di assistenza e privacy è passato a `info@ifgecommerce.com`.

**Link Coach — Grafo di collegamenti interni** — Nuova analisi di quanto i prodotti sono collegati tra loro tramite collezioni condivise, vendor e tag, con suggerimenti spiegabili e un riepilogo in Dashboard.

**Matrice di prontezza** — La Dashboard ha guadagnato un unico pannello a colpo d'occhio che aggrega ogni segnale GEO tracciato dall'app: estraibilità del contenuto, schema Organization, `llms.txt`, `agents.md`, accesso crawler, prontezza MCP, connettività Link Coach e (una volta rilasciato) traffico da citazioni AI.

**Motore di riscrittura contenuti** — Aggiunto uno strumento assistito da AI per riscrivere la descrizione di un prodotto rendendola più densa di fatti verificabili e più facile da citare per un motore generativo, con una revisione prima/dopo obbligatoria prima che qualcosa venga scritto sul prodotto.

**Confronto competitivo** — Incolla l'URL di un prodotto competitor e vedi gli stessi segnali GEO messi a confronto fianco a fianco con il tuo prodotto.

**Tracking visibilità AI** — Verifiche settimanali automatiche se Claude, ChatGPT, Gemini e Perplexity citano il tuo negozio sulle domande che scegli di monitorare, con un grafico di andamento e un dettaglio per motore.

**Schema Organization e `agents.md`** — Aggiunti dati strutturati sull'identità aziendale (ragione sociale, P.IVA, indirizzo) per i sistemi AI che verificano che un'azienda sia reale, e un file `agents.md` generato che descrive il negozio agli agenti di acquisto autonomi.

**Fatturazione** — I negozianti possono sottoscrivere Grow o Unlimited, con fatturazione mensile o annuale, direttamente dalla pagina Piani, e tornare a Free in qualsiasi momento senza contattare l'assistenza.

**Revisione privacy policy e conformità App Store** — Pubblicato questo centro assistenza e una privacy policy formale; confermato che i permessi Shopify dell'app e la gestione dei webhook GDPR soddisfano i requisiti dell'App Store in vista della sottomissione.

**Generazione FAQ assistita da AI** — Genera tre-cinque coppie domanda-risposta per prodotto a partire da titolo, descrizione e specifiche già esistenti, rivedile e pubblica quelle approvate. Le FAQ pubblicate compaiono sulla pagina prodotto e come dati strutturati `FAQPage`.

**Punteggio di estraibilità dei contenuti (chunking)** — L'audit del catalogo valuta anche quanto sia facile per un sistema AI estrarre e citare la descrizione di ogni prodotto — non solo se i campi di dati strutturati sono presenti, ma se il testo stesso è utilizzabile.

**Simulatore crawler** — Recupera qualsiasi pagina prodotto esattamente come la vede un crawler AI — senza JavaScript, come GPTBot, ClaudeBot e PerplexityBot — inclusi i controlli di robots.txt per singolo bot.

**Audit del catalogo e correzioni con un clic** — Lanciato l'audit principale: analizza il catalogo rispetto a nove campi di dati strutturati, assegna un punteggio a ogni prodotto e corregge in modo sicuro con un clic ciò che può. Aggiunta anche la generazione reale di `llms.txt`, servito sulla vera root del negozio.

## Versioni precedenti

Rilascio iniziale: configurazione dell'app embedded, autenticazione Shopify e infrastruttura dati di base.

[← Torna al Centro Assistenza](index.html)
