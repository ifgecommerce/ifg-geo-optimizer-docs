---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
---

# Privacy Policy

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <span class="lang-item lang-current"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</span>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

**IFG GEO Optimizer** — un'app Shopify per la Generative Engine Optimization
Ultimo aggiornamento: luglio 2026

## 1. Titolare del trattamento

Il titolare del trattamento dei dati personali processati tramite **IFG GEO Optimizer** è:

**IFG eCommerce**
Con sede a Roma, Italia
Email: [ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

## 2. Cosa raccogliamo

- **Dati account del negoziante (tramite Shopify OAuth)**: il dominio del tuo negozio, un token di accesso API e l'indirizzo email associato al tuo account Shopify.
- **Dati del catalogo (sola lettura)**: titoli prodotto, descrizioni, marchio, prezzi, opzioni e specifiche tecniche — usati per eseguire audit, simulare il comportamento dei crawler, valutare l'estraibilità dei contenuti e generare bozze di FAQ.
- **Configurazione del negozio**: il tuo piano attivo, i dettagli della politica di reso e di spedizione che inserisci in Impostazioni, e qualunque bozza o approvazione di FAQ che crei.
- **Dati tecnici**: timestamp delle richieste, identificativi interni dei record e log di sistema.

> L'app non richiede né riceve mai dati dei clienti finali — niente nomi, email, indirizzi o ordini. Gli unici permessi Shopify richiesti sono `read_products` e `write_products`.

## 3. Perché li trattiamo, e su quale base giuridica

Trattiamo questi dati per fornire il servizio per cui hai installato l'app — ai sensi dell'Art. 6(1)(b) GDPR, esecuzione di un contratto: analizzare e migliorare la visibilità del tuo catalogo sui motori di ricerca generativi (ChatGPT, Perplexity, Gemini, Google AI Overviews), inclusa la generazione di FAQ quando lo richiedi esplicitamente.

## 4. Come li raccogliamo

I dati dell'account vengono raccolti una sola volta, tramite il flusso OAuth di Shopify, al momento dell'installazione dell'app. I dati del catalogo vengono letti tramite l'Admin API di Shopify solo quando avvii un'azione — una scansione, una simulazione o una generazione di FAQ — dalla dashboard dell'app. Nulla viene eseguito in background senza una tua richiesta esplicita.

## 5. Con chi li condividiamo

- **Google Firebase / Cloud Firestore** — memorizza la configurazione del tuo negozio, le sessioni e le bozze di FAQ. Google LLC (USA) aderisce al Data Privacy Framework UE-USA. I dati sono conservati nella regione europe-west1 (Belgio).
- **Anthropic PBC (USA)** — fornisce il modello linguistico (Claude) usato per generare le bozze di FAQ, solo quando richiedi esplicitamente una generazione. Riceve solo gli attributi prodotto che hai già inserito — titolo, descrizione, marchio, specifiche — mai dati dei clienti. Consulta la privacy policy e i termini commerciali di Anthropic per sapere come gestiscono quei dati.
- **Shopify Inc.** — la piattaforma stessa, e la fonte dell'Admin API che l'app utilizza.

Non vendiamo dati, e non li usiamo per marketing o profilazione comportamentale.

## 6. Per quanto tempo li conserviamo

- **Token di sessione**: gestiti dal ciclo di vita dei token offline di Shopify, rinnovati automaticamente.
- **Configurazione, audit e bozze di FAQ**: conservati per tutta la durata dell'installazione dell'app. La disinstallazione attiva il webhook `shop/redact` di Shopify, che elimina completamente la configurazione e le sessioni del tuo negozio.
- **Log tecnici**: conservati secondo la politica di conservazione standard dei log di Google Cloud.

## 7. I tuoi diritti

Ai sensi degli Articoli 15–22 GDPR, puoi richiedere l'accesso ai tuoi dati, la correzione di dati inesatti o la cancellazione — il modo più semplice è disinstallare l'app — oppure opporti al trattamento. Puoi anche presentare un reclamo alla tua autorità di controllo locale per la protezione dei dati. Poiché l'app non tratta mai dati dei clienti finali, i webhook di conformità `customers/data_request` e `customers/redact` rispondono confermando che non c'è nulla da esportare o cancellare.

## 8. Sicurezza

Tutto il traffico avviene su HTTPS/TLS 1.2+. I token di autenticazione Shopify non sono mai esposti al browser. Ogni webhook viene verificato con un controllo HMAC SHA-256 a tempo costante prima di essere elaborato. Il database è raggiungibile solo dal backend, autenticato tramite l'identità del servizio della piattaforma di hosting — non ci sono credenziali statiche nel codice, e l'accesso diretto dal client è negato dalle regole di sicurezza del database stesso. I dati sono crittografati sia a riposo che in transito.

## 9. Modifiche

Potremmo aggiornare questa policy di tanto in tanto. Le modifiche sostanziali saranno riportate qui, con la data in cima sempre aggiornata.

---

**Domande sui tuoi dati?**
[ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

[← Torna al Centro Assistenza](index.html)
