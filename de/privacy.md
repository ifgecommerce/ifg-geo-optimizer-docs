---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
---

# Privacy Policy

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <span class="lang-item lang-current"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</span>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

**IFG GEO Optimizer** — eine Shopify-App für Generative Engine Optimization
Zuletzt aktualisiert: Juli 2026

## 1. Verantwortlicher für die Datenverarbeitung

Verantwortlicher für die im Rahmen von **IFG GEO Optimizer** verarbeiteten personenbezogenen Daten ist:

**IFG eCommerce**
Mit Sitz in Rom, Italien
E-Mail: [ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

## 2. Welche Daten wir erfassen

- **Händler-Kontodaten (über Shopify OAuth)**: Ihre Shop-Domain, ein API-Zugriffstoken und die E-Mail-Adresse Ihres Shopify-Kontos.
- **Katalogdaten (nur Lesezugriff)**: Produkttitel, Beschreibungen, Hersteller, Preise, Optionen und technische Spezifikationen — verwendet, um Audits durchzuführen, das Crawler-Verhalten zu simulieren, die Extrahierbarkeit von Inhalten zu bewerten und FAQs zu entwerfen.
- **Shop-Konfiguration**: Ihr aktiver Plan, die in den Einstellungen hinterlegten Rückgabe- und Versandrichtlinien sowie alle von Ihnen erstellten FAQ-Entwürfe und Freigaben.
- **Technische Daten**: Zeitstempel von Anfragen, interne Datensatz-Kennungen und Systemprotokolle.

> Die App fordert oder erhält niemals Daten von Endkunden — keine Namen, E-Mail-Adressen, Adressen oder Bestellungen. Die einzigen angeforderten Shopify-Berechtigungen sind `read_products` und `write_products`.

## 3. Warum wir diese Daten verarbeiten und auf welcher Rechtsgrundlage

Wir verarbeiten diese Daten, um die Dienstleistung zu erbringen, für die Sie die App installiert haben — auf Grundlage von Art. 6 Abs. 1 lit. b DSGVO (Erfüllung eines Vertrags): Analyse und Verbesserung der Sichtbarkeit Ihres Katalogs auf generativen Suchmaschinen (ChatGPT, Perplexity, Gemini, Google AI Overviews), einschließlich der Erstellung von FAQ-Entwürfen, wenn Sie dies ausdrücklich anfordern.

## 4. Wie wir die Daten erfassen

Kontodaten werden einmalig über den OAuth-Ablauf von Shopify erfasst, wenn Sie die App installieren. Katalogdaten werden nur über die Admin-API von Shopify gelesen, wenn Sie eine Aktion auslösen — einen Scan, eine Simulation oder eine FAQ-Generierung — vom Dashboard der App aus. Nichts läuft im Hintergrund, ohne dass Sie es angefordert haben.

## 5. An wen wir die Daten weitergeben

- **Google Firebase / Cloud Firestore** — speichert Ihre Shop-Konfiguration, Sitzungen und FAQ-Entwürfe. Google LLC (USA) nimmt am EU-US Data Privacy Framework teil. Die Daten werden in der Region europe-west1 (Belgien) gespeichert.
- **Anthropic PBC (USA)** — stellt das Sprachmodell (Claude) bereit, das für die Erstellung von FAQ-Vorschlägen verwendet wird, nur wenn Sie ausdrücklich eine Generierung anfordern. Es erhält ausschließlich die von Ihnen bereits eingegebenen Produktattribute — Titel, Beschreibung, Hersteller, Spezifikationen — niemals Kundendaten. Wie Anthropic mit diesen Daten umgeht, entnehmen Sie der eigenen Datenschutzerklärung und den Geschäftsbedingungen von Anthropic.
- **Shopify Inc.** — die Plattform selbst und die Quelle der Admin-API, die die App nutzt.

Wir verkaufen keine Daten und verwenden sie nicht für Marketing oder Verhaltensprofiling.

## 6. Wie lange wir die Daten aufbewahren

- **Sitzungstoken**: verwaltet durch den Offline-Token-Lebenszyklus von Shopify, automatisch rotiert.
- **Konfiguration, Audits und FAQ-Entwürfe**: aufbewahrt, solange die App installiert ist. Eine Deinstallation löst den `shop/redact`-Webhook von Shopify aus, der die Konfiguration und Sitzungen Ihres Shops vollständig löscht.
- **Technische Protokolle**: aufbewahrt gemäß der Standard-Protokollierungsaufbewahrung von Google Cloud.

## 7. Ihre Rechte

Gemäß Art. 15–22 DSGVO können Sie Auskunft über Ihre Daten, die Berichtigung unrichtiger Daten oder die Löschung verlangen — am einfachsten durch Deinstallation der App — oder der Verarbeitung widersprechen. Sie können außerdem eine Beschwerde bei Ihrer zuständigen Datenschutzbehörde einreichen. Da die App niemals Daten von Endkunden verarbeitet, bestätigen die Compliance-Webhooks `customers/data_request` und `customers/redact`, dass nichts zu exportieren oder zu löschen ist.

## 8. Sicherheit

Der gesamte Datenverkehr läuft über HTTPS/TLS 1.2+. Shopify-Authentifizierungstoken werden dem Browser nie offengelegt. Jeder Webhook wird vor der Verarbeitung mit einer zeitkonstanten HMAC-SHA-256-Prüfung verifiziert. Die Datenbank ist ausschließlich über die eigene Serviceidentität des Backends der Hosting-Plattform erreichbar — es gibt keine statischen Zugangsdaten im Code, und direkter Client-Zugriff wird durch die eigenen Sicherheitsregeln der Datenbank verweigert. Daten werden verschlüsselt gespeichert und übertragen.

## 9. Änderungen

Wir können diese Richtlinie von Zeit zu Zeit aktualisieren. Wesentliche Änderungen werden hier abgebildet, das Datum oben wird stets aktuell gehalten.

---

**Fragen zu Ihren Daten?**
[ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

[← Zurück zum Hilfe-Center](index.html)
