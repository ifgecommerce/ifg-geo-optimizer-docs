---
title: IFG GEO Optimizer
description: Documentazione, FAQ e pagine legali per l'app Shopify IFG GEO Optimizer.
lang: it
---

# Domande Frequenti

<div class="lang-switcher">
{% include lang-switcher.html current="it" slug="faq" %}
</div>

**Qual è la differenza tra GEO e SEO?**
La SEO tradizionale ottimizza per i motori di ricerca che classificano ed elencano link. La GEO (Generative Engine Optimization) ottimizza per i sistemi AI che leggono i tuoi contenuti e generano direttamente una risposta o un consiglio — ChatGPT, Perplexity, Gemini, Claude e Google AI Overviews. Le due discipline si sovrappongono, ma la GEO si occupa di aspetti che gli strumenti SEO classici non verificano: se la tua pagina prodotto ha dati strutturati completi, se un crawler AI riesce davvero a leggere i tuoi contenuti senza eseguire JavaScript, e se i tuoi testi sono scritti in un modo facile da citare e riportare.

**L'app accede mai ai dati dei miei clienti?**
Nessun dato personale dei clienti. I permessi Shopify dell'app sono `read_products`, `write_products`, `read_themes` e `write_pixels` — leggere e migliorare il catalogo, verificare che il blocco tema sia attivo, e attivare un pixel anonimo di traffico storefront (vedi sotto). Non richiede mai accesso a ordini o dati clienti. Consulta la [Privacy Policy](privacy.html) per il dettaglio completo.

**Cos'è il pixel di traffico da citazioni AI, e traccia i miei clienti?**
Su Grow e Unlimited, un piccolo Web Pixel rileva quando una visita al negozio arriva da un motore AI noto (tramite il referrer del browser) e registra il motore, la pagina e un timestamp — nulla che identifichi il visitatore, nessun cookie, nessun dato di sessione. Gira solo se il visitatore ha già dato il consenso all'analisi tramite il banner cookie del negozio (Customer Privacy API di Shopify). Alimenta un tile della Dashboard ("Traffico da citazioni AI, ultimi 7 giorni") — il complemento del tracking Visibilità AI, che dice se sei citato ma non se quella citazione porta traffico.

**Cosa cambia davvero il pulsante "Correggi" nell'audit catalogo?**
Scrive i dati strutturati schema.org mancanti in un metafield del prodotto — cose come le specifiche tecniche derivate dalle opzioni prodotto già esistenti. Non tocca mai il titolo, la descrizione, le immagini o il prezzo del tuo prodotto, e non inventa mai dati che non può verificare: un codice a barre mancante, ad esempio, resta mancante invece di essere indovinato.

**Le FAQ e le descrizioni riscritte sono inventate dall'AI o basate sul mio prodotto reale?**
Il modello vede solo i dati prodotto che hai già — titolo, descrizione, marchio e specifiche tecniche — e riceve istruzioni esplicite di non aggiungere nulla che non sia presente in quei dati. Rivedi ogni FAQ o descrizione riscritta prima che venga pubblicata; nulla va online automaticamente.

**Cosa succede ai miei dati se disinstallo l'app?**
La configurazione del tuo negozio, gli audit salvati, le bozze di FAQ e riscrittura contenuti, i prompt di visibilità e gli eventi di traffico da citazioni AI vengono eliminati automaticamente quando Shopify ci notifica la disinstallazione. L'app non trattiene nulla dopo che te ne sei andato.

**Posso annullare o effettuare il downgrade senza contattare l'assistenza?**
Sì. Vai su **Piani** dentro l'app e passa a Free in qualsiasi momento — ha effetto immediato, nessuna email richiesta.

## Limiti dei piani

| Funzione | Free | Grow | Unlimited |
|---|---|---|---|
| Audit catalogo | Primi 20 prodotti, una tantum, no storico | Catalogo intero + storico | Catalogo intero + storico |
| Crawler simulator | 20/mese | 300/mese | 1.000/mese |
| Confronto competitivo | 10/mese | 50/mese | 150/mese |
| Generazione FAQ | Non incluso | 500/mese | 500/mese |
| Riscrittura contenuti | Non incluso | 300/mese | 300/mese |
| Visibilità AI (domande monitorate) | Non incluso | 5 domande | 15 domande |
| Pixel traffico da citazioni AI | Non incluso | Incluso | Incluso |
| Chat di assistenza AI | 1.000 messaggi/mese | 1.000 messaggi/mese | 1.000 messaggi/mese |
| Lingue interfaccia | Tutte e 30 | Tutte e 30 | Tutte e 30 |

Prezzo mensile: Free $0, Grow $9,99, Unlimited $19,99. La fatturazione annuale su Grow/Unlimited equivale a circa due mesi gratis rispetto al mensile.

**Perché il piano Free copre solo 20 prodotti?**
Serve a farti vedere risultati reali sul tuo catalogo prima di passare a un piano a pagamento. Grow e Unlimited rimuovono questo limite e conservano lo storico completo degli audit passati.

**C'è davvero un tetto alla generazione FAQ anche su Unlimited?**
Sì — 500 generazioni al mese, deliberatamente, anche sul piano più alto. Questo mantiene la funzionalità sostenibile al prezzo attuale; se hai un catalogo ad alto volume e ti serve di più, contattaci e troviamo una soluzione.

**Perché la chat di assistenza AI è uguale su ogni piano?**
È una scelta di prodotto, non una dimenticanza: l'assistenza è inclusa per tutti, mai un differenziatore a pagamento. Il tetto di messaggi (1.000/mese) esiste solo come freno tecnico contro gli abusi, non come limite reale — nessun uso legittimo si avvicina a quella soglia.

**Ho trovato un bug o qualcosa non sembra funzionare bene. A chi lo segnalo?**
Scrivi a [info@ifgecommerce.com](mailto:info@ifgecommerce.com) descrivendo cosa hai visto e, se puoi, quale prodotto o pagina era coinvolta — di solito è sufficiente per individuare rapidamente il problema. Puoi anche usare la chat di assistenza AI nell'app e chiedere di parlare con una persona.

[← Torna al Centro Assistenza](index.html)
