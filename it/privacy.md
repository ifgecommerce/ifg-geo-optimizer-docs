---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
lang: it
---

# Privacy Policy

<div class="lang-switcher">
{% include lang-switcher.html current="it" slug="privacy" %}
</div>

**IFG GEO Optimizer** — un'app Shopify per la Generative Engine Optimization
Ultimo aggiornamento: luglio 2026

## 1. Titolare del trattamento

Il titolare del trattamento dei dati personali processati tramite **IFG GEO Optimizer** è:

**IFG eCommerce** — con sede a Roma, Italia
Email: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Cosa raccogliamo

- **Dati account del negoziante (tramite Shopify OAuth)**: il dominio del tuo negozio, un token di accesso API e l'indirizzo email associato al tuo account Shopify.
- **Dati del catalogo (sola lettura)**: titoli prodotto, descrizioni, marchio, prezzi, opzioni e specifiche tecniche — usati per eseguire audit, simulare il comportamento dei crawler, valutare l'estraibilità dei contenuti e generare bozze di FAQ o descrizioni riscritte.
- **Configurazione del negozio**: il tuo piano attivo, i dettagli della politica di reso/spedizione e i dati aziendali che inserisci in Impostazioni, gli audit salvati, le bozze di FAQ e riscrittura contenuti, e le domande che scegli di monitorare per la visibilità AI.
- **Messaggi della chat di assistenza**: il testo che scambi con l'assistente AI integrato nell'app, inclusa la trascrizione inoltrata a noi se chiedi esplicitamente di parlare con una persona.
- **Traffico storefront anonimo (Web Pixel, Grow/Unlimited)**: quando un visitatore arriva su una pagina prodotto a partire da un motore AI riconosciuto (ChatGPT, Perplexity, Claude, Gemini, Copilot), registriamo il motore, l'URL della pagina e un timestamp — solo se il visitatore ha già dato il consenso all'analisi tramite il banner cookie del tuo negozio. Nessun identificativo del visitatore, cookie o dato di sessione viene raccolto.
- **Dati tecnici**: timestamp delle richieste, identificativi interni dei record e log di sistema.

> L'app **non richiede né riceve mai dati personali dei clienti finali** — niente nomi, email, indirizzi o ordini. I permessi Shopify richiesti sono `read_products`, `write_products` (catalogo e dati strutturati), `read_themes` (verifica che il blocco tema sia attivo) e `write_pixels` (attivazione del pixel anonimo di traffico sopra descritto).

## 3. Perché li trattiamo, e su quale base giuridica

Trattiamo questi dati per fornire il servizio per cui hai installato l'app — ai sensi dell'Art. 6(1)(b) GDPR, esecuzione di un contratto: analizzare e migliorare la visibilità del tuo catalogo sui motori di ricerca generativi, inclusa la generazione assistita di FAQ e la riscrittura contenuti, la chat di assistenza integrata, il tracking settimanale della visibilità AI sulle domande che scegli, e la misurazione anonima del traffico da citazioni AI — sempre su iniziativa del negoziante o, per il pixel di traffico, subordinata al consenso sullo storefront.

## 4. Come li raccogliamo

I dati dell'account vengono raccolti una sola volta, tramite il flusso OAuth di Shopify, al momento dell'installazione. I dati del catalogo vengono letti tramite l'Admin API di Shopify solo quando avvii un'azione dalla dashboard. Il pixel di traffico gira sul tuo storefront e registra eventi solo dopo il consenso; nient'altro viene eseguito in background senza una tua richiesta esplicita.

## 5. Con chi li condividiamo

- **Google Firebase / Cloud Firestore** — memorizza la tua configurazione, le sessioni e le bozze. Google LLC (USA) aderisce al Data Privacy Framework UE-USA. Dati conservati nella regione europe-west1 (Belgio).
- **Anthropic PBC (USA)** — fornisce il modello Claude usato per la generazione FAQ, la riscrittura contenuti e la chat di assistenza integrata, solo su tua azione esplicita. Riceve solo gli attributi prodotto o il testo della chat che fornisci — mai dati dei clienti.
- **OpenAI, Inc. (USA)** e **Perplexity AI, Inc. (USA)** — usati esclusivamente per il tracking settimanale della visibilità AI sulle domande che scegli esplicitamente di monitorare. Ricevono solo il testo della domanda tracciata — mai dati dei clienti.
- **Google LLC (USA)** — fornisce il modello Gemini, usato allo stesso modo di OpenAI/Perplexity sopra per il tracking visibilità (uso distinto da Firebase/Firestore, che riguarda solo l'archiviazione).
- **Resend, Inc. (USA)** — ci invia una notifica, con il nome del negozio e la trascrizione della chat di assistenza, solo quando chiedi esplicitamente di parlare con una persona nella chat.
- **Shopify Inc.** — la piattaforma stessa, e la fonte dell'Admin API e dell'infrastruttura Web Pixel che l'app utilizza.

Non vendiamo dati, e non li usiamo per marketing o profilazione comportamentale.

## 6. Per quanto tempo li conserviamo

- **Token di sessione**: gestiti dal ciclo di vita dei token offline di Shopify, rinnovati automaticamente.
- **Configurazione, audit, bozze ed eventi di traffico**: conservati per tutta la durata dell'installazione dell'app. La disinstallazione attiva il webhook `shop/redact` di Shopify, che elimina completamente la configurazione e le sessioni del tuo negozio.
- **Log tecnici**: conservati secondo la politica di conservazione standard dei log di Google Cloud.

## 7. I tuoi diritti

Ai sensi degli Articoli 15–22 GDPR, puoi richiedere l'accesso ai tuoi dati, la correzione di dati inesatti o la cancellazione — il modo più semplice è disinstallare l'app — oppure opporti al trattamento. Puoi anche presentare un reclamo alla tua autorità di controllo locale per la protezione dei dati. Poiché l'app non tratta mai dati personali dei clienti finali, i webhook di conformità `customers/data_request` e `customers/redact` rispondono confermando che non c'è nulla da esportare o cancellare.

## 8. Sicurezza

Tutto il traffico avviene su HTTPS/TLS 1.2+. I token di autenticazione Shopify non sono mai esposti al browser. Ogni webhook viene verificato con un controllo HMAC SHA-256 a tempo costante prima di essere elaborato. Il database è raggiungibile solo dal backend, autenticato tramite l'identità del servizio della piattaforma di hosting — non ci sono credenziali statiche nel codice, e l'accesso diretto dal client è negato dalle regole di sicurezza del database stesso. I dati sono crittografati sia a riposo che in transito.

## 9. Modifiche

Potremmo aggiornare questa policy di tanto in tanto. Le modifiche sostanziali saranno riportate qui, con la data in cima sempre aggiornata.

---

**Domande sui tuoi dati?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Torna al Centro Assistenza](index.html)
