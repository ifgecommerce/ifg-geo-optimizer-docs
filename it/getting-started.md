---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
---

# Guida introduttiva

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <span class="lang-item lang-current"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</span>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

Questa guida copre tutto, dall'installazione dell'app alla pubblicazione della tua prima FAQ ottimizzata per l'AI.

## 1. Installa e apri la dashboard

Una volta installata, IFG GEO Optimizer si apre dentro il tuo admin Shopify. La dashboard è la tua base operativa — si popola con il punteggio GEO del tuo negozio e l'attività recente man mano che usi l'app.

## 2. Compila le tue politiche

Vai su **Impostazioni** e inserisci i dettagli della tua politica di reso e di spedizione (finestra di reso, chi paga la spedizione di reso, tempi di gestione e di transito, paese di destinazione). Questi dati alimentano direttamente i dati strutturati che l'app pubblica per ogni prodotto — le pagine prodotto di Shopify non espongono queste informazioni ai motori di ricerca in altro modo, quindi questo solo passaggio migliora in modo misurabile il tuo punteggio di audit.

## 3. Esegui il tuo primo audit del catalogo

Apri **Audit catalogo** e clicca su **Riesegui scansione catalogo**. L'app legge il tuo catalogo prodotti tramite l'Admin API di Shopify e controlla ogni prodotto rispetto a nove campi di dati strutturati che i motori di ricerca cercano: immagine, descrizione, marchio, SKU, GTIN, prezzo, specifiche tecniche, politica di reso e politica di spedizione.

I prodotti sotto 80/100 mostrano esattamente cosa manca. Dove l'app può correggere automaticamente — di solito derivando le specifiche tecniche dalle opzioni prodotto già esistenti — vedrai un pulsante **Correggi**. Un clic scrive direttamente sul prodotto i dati schema.org mancanti; nulla viene indovinato o inventato per i campi che l'app non può derivare in modo sicuro (un codice a barre, ad esempio, non viene mai generato automaticamente).

Sul piano Free, gli audit coprono i primi 20 prodotti e non conservano storico. Grow e Unlimited coprono l'intero catalogo e salvano ogni scansione.

## 4. Attiva il blocco tema

I dati strutturati corretti dal tuo audit non compaiono sul tuo storefront finché non li attivi. Nell'editor del tuo tema, vai su **Incorporamenti app** e attiva **GEO Schema**. È un'attivazione una tantum — da quel momento, ogni pagina prodotto include automaticamente il JSON-LD generato dal tuo audit.

## 5. Controlla cosa vede davvero un bot

Apri **Crawler AI** e scegli un prodotto. L'app recupera la pagina esattamente come farebbe un crawler AI — senza esecuzione di JavaScript, come GPTBot, ClaudeBot o PerplexityBot — così puoi vedere con precisione cosa è visibile a questi motori, incluso se il tuo robots.txt li sta bloccando e se i tuoi dati strutturati sono completi nell'HTML grezzo.

## 6. Genera le FAQ

Su Grow o Unlimited, apri **FAQ prodotto**, scegli un prodotto e clicca su **Genera 3 FAQ**. L'app scrive tre coppie domanda-risposta a partire dal titolo, dalla descrizione e dalle specifiche effettive del tuo prodotto — mai dettagli inventati. Rivedi ogni bozza, poi clicca su **Approva e pubblica** per quelle che vuoi rendere live; le FAQ approvate compaiono sulla pagina prodotto e vengono marcate come dati strutturati FAQPage per i motori di ricerca. Nulla viene pubblicato senza la tua revisione.

## 7. Scegli un piano

**Prezzi** mostra Free, Grow e Unlimited a confronto, con fatturazione mensile e annuale. Puoi cambiare piano o tornare a Free in qualsiasi momento, direttamente dall'app — senza bisogno di contattare l'assistenza per effettuare il downgrade.

Questo è il ciclo completo. La maggior parte dei negozianti riesegue un audit dopo aver aggiunto nuovi prodotti, e controlla il simulatore crawler ogni volta che aggiorna una descrizione prodotto.

[← Torna al Centro Assistenza](index.html)
