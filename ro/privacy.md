---
title: IFG GEO Optimizer
description: Documentație, întrebări frecvente și pagini legale pentru aplicația Shopify IFG GEO Optimizer.
lang: ro
---

# Politica de confidențialitate

<div class="lang-switcher">
{% include lang-switcher.html current="ro" slug="privacy" %}
</div>

**IFG GEO Optimizer** — o aplicație Shopify pentru Generative Engine Optimization
Ultima actualizare: iulie 2026

## 1. Operatorul de date

Operatorul de date pentru datele cu caracter personal prelucrate prin **IFG GEO Optimizer** este:

**IFG eCommerce** — cu sediul în Roma, Italia
Email: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Ce colectăm

- **Datele contului comerciantului (prin Shopify OAuth)**: domeniul magazinului tău, un token de acces API și adresa de email de pe contul tău Shopify.
- **Date de catalog (doar citire)**: titluri de produse, descrieri, furnizor, prețuri, opțiuni și specificații tehnice — folosite pentru a rula audituri, a simula comportamentul crawler-elor, a evalua extractibilitatea conținutului și a redacta FAQ-uri sau descrieri rescrise.
- **Configurația magazinului**: planul tău activ, detaliile politicii de retur și livrare și datele companiei pe care le introduci în Setări, auditurile salvate, ciornele de FAQ și rescriere de conținut, precum și prompt-urile pe care alegi să le urmărești pentru vizibilitatea AI.
- **Mesaje de chat de asistență**: textul pe care îl schimbi cu asistentul AI din aplicație, inclusiv transcrierea trimisă către noi dacă ceri explicit să vorbești cu un om.
- **Trafic anonim pe magazinul vitrină (Web Pixel, Grow/Unlimited)**: când un vizitator ajunge pe o pagină de produs de la un motor AI recunoscut (ChatGPT, Perplexity, Claude, Gemini, Copilot), înregistrăm motorul, URL-ul paginii și o marcă temporală — doar dacă vizitatorul a acordat deja consimțământul de analiză prin bannerul de cookie-uri al magazinului tău. Nu se colectează niciun identificator de vizitator, cookie sau date de sesiune.
- **Date tehnice**: mărci temporale ale cererilor, identificatori interni de înregistrări și jurnale de sistem.

> Aplicația **nu solicită și nu primește niciodată date personale ale clienților finali** — fără nume, emailuri, adrese sau comenzi. Permisiunile Shopify solicitate sunt `read_products`, `write_products` (catalog și date structurate), `read_themes` (verificarea că embed-ul temei este activ) și `write_pixels` (activarea pixelului anonim de trafic de mai sus).

## 3. De ce le prelucrăm și pe ce bază legală

Prelucrăm aceste date pentru a furniza serviciul pentru care ai instalat aplicația — în temeiul Art. 6(1)(b) GDPR, executarea unui contract: analizarea și îmbunătățirea vizibilității catalogului tău pe motoarele de căutare generative, inclusiv redactarea de FAQ asistată de AI și rescrierea conținutului, chatul de asistență din aplicație, urmărirea săptămânală a vizibilității AI pe prompt-urile pe care le alegi și măsurarea anonimă a traficului de recomandare AI — toate fie inițiate de comerciant, fie, în cazul pixelului de trafic, condiționate de consimțământ pe magazinul tău vitrină.

## 4. Cum le colectăm

Datele contului sunt colectate o singură dată, prin fluxul OAuth al Shopify, la instalare. Datele de catalog sunt citite prin Admin API al Shopify doar când declanșezi o acțiune din dashboard. Pixelul de trafic rulează pe magazinul tău vitrină și raportează evenimente doar după consimțământ; nimic altceva nu rulează în fundal fără să ceri tu.

## 5. Cu cine le partajăm

- **Google Firebase / Cloud Firestore** — stochează configurația, sesiunile și ciornele tale. Google LLC (SUA) participă la EU-US Data Privacy Framework. Datele sunt stocate în regiunea europe-west1 (Belgia).
- **Anthropic PBC (SUA)** — furnizează modelul Claude folosit pentru redactarea FAQ-urilor, rescrierea conținutului și chatul de asistență din aplicație, doar la acțiunea ta explicită. Primește doar atributele de produs sau textul de chat pe care le furnizezi — niciodată date despre clienți.
- **OpenAI, Inc. (SUA)** și **Perplexity AI, Inc. (SUA)** — folosite exclusiv pentru urmărirea săptămânală a vizibilității AI pe prompt-urile pe care alegi explicit să le monitorizezi. Primesc doar textul prompt-ului urmărit — niciodată date despre clienți.
- **Google LLC (SUA)** — furnizează modelul Gemini, folosit în același mod ca OpenAI/Perplexity de mai sus pentru urmărirea vizibilității (o utilizare distinctă de Firebase/Firestore, care este doar stocare).
- **Resend, Inc. (SUA)** — ne trimite o notificare, cu numele magazinului și transcrierea chatului de asistență, doar când ceri explicit să vorbești cu un om în chatul de asistență.
- **Shopify Inc.** — platforma în sine și sursa infrastructurii Admin API și Web Pixel folosite de aplicație.

Nu vindem date și nu le folosim pentru marketing sau profilare comportamentală.

## 6. Cât timp le păstrăm

- **Token-uri de sesiune**: gestionate de ciclul de viață al token-urilor offline al Shopify, rotite automat.
- **Configurație, audituri, ciorne și evenimente de trafic**: păstrate atât timp cât aplicația este instalată. Dezinstalarea declanșează webhook-ul `shop/redact` al Shopify, care șterge complet configurația și sesiunile magazinului tău.
- **Jurnale tehnice**: păstrate conform politicii standard de retenție a jurnalelor Google Cloud.

## 7. Drepturile tale

În temeiul articolelor 15–22 GDPR, poți solicita accesul la datele tale, corectarea datelor inexacte sau ștergerea — cel mai simplu mod este dezinstalarea aplicației — sau te poți opune prelucrării. Poți depune și o plângere la autoritatea locală de protecție a datelor. Deoarece aplicația nu prelucrează niciodată date personale ale clienților finali, webhook-urile de conformitate `customers/data_request` și `customers/redact` răspund confirmând că nu există nimic de exportat sau șters.

## 8. Securitate

Tot traficul rulează prin HTTPS/TLS 1.2+. Token-urile de autentificare Shopify nu sunt niciodată expuse browserului. Fiecare webhook este verificat cu o verificare HMAC SHA-256 în timp constant înainte de a fi procesat. Baza de date este accesibilă doar din backend, autentificată prin identitatea proprie de serviciu a platformei de găzduire — nu există credențiale statice în cod, iar accesul direct al clientului este refuzat de regulile proprii de securitate ale bazei de date. Datele sunt criptate atât în repaus, cât și în tranzit.

## 9. Modificări

Este posibil să actualizăm această politică din când în când. Modificările substanțiale vor fi reflectate aici, cu data din partea de sus menținută actualizată.

---

**Întrebări despre datele tale?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Înapoi la Centrul de asistență](index.html)
