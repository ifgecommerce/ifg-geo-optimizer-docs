---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
lang: de
---

# Privacy Policy

<div class="lang-switcher">
{% include lang-switcher.html current="de" slug="privacy" %}
</div>

**IFG GEO Optimizer** — eine Shopify-App für Generative Engine Optimization
Zuletzt aktualisiert: Juli 2026

## 1. Verantwortlicher für die Datenverarbeitung

Verantwortlicher für die im Rahmen von **IFG GEO Optimizer** verarbeiteten personenbezogenen Daten ist:

**IFG eCommerce** — mit Sitz in Rom, Italien
E-Mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Welche Daten wir erfassen

- **Händler-Kontodaten (über Shopify OAuth)**: Ihre Shop-Domain, ein API-Zugriffstoken und die E-Mail-Adresse Ihres Shopify-Kontos.
- **Katalogdaten (nur Lesezugriff)**: Produkttitel, Beschreibungen, Hersteller, Preise, Optionen und technische Spezifikationen — verwendet, um Audits durchzuführen, das Crawler-Verhalten zu simulieren, die Extrahierbarkeit von Inhalten zu bewerten und FAQs oder umgeschriebene Beschreibungen zu entwerfen.
- **Shop-Konfiguration**: Ihr aktiver Plan, die in den Einstellungen hinterlegten Rückgabe- und Versandrichtlinien und Unternehmensdaten, gespeicherte Audits, FAQ- und Content-Rewrite-Entwürfe sowie die Prompts, die Sie für das KI-Visibility-Tracking auswählen.
- **Support-Chat-Nachrichten**: der Text, den Sie mit dem KI-Assistenten in der App austauschen, einschließlich des an uns weitergeleiteten Transkripts, wenn Sie ausdrücklich bitten, mit einem Menschen zu sprechen.
- **Anonymer Storefront-Traffic (Web Pixel, Grow/Unlimited)**: Wenn ein Besucher über eine bekannte KI-Engine (ChatGPT, Perplexity, Claude, Gemini, Copilot) auf einer Produktseite ankommt, erfassen wir die Engine, die Seiten-URL und einen Zeitstempel — nur, wenn der Besucher bereits über den Cookie-Banner Ihres Shops der Analyse zugestimmt hat. Es werden keine Besucherkennung, Cookies oder Sitzungsdaten erfasst.
- **Technische Daten**: Zeitstempel von Anfragen, interne Datensatz-Kennungen und Systemprotokolle.

> Die App fordert oder erhält **niemals personenbezogene Daten von Endkunden** — keine Namen, E-Mail-Adressen, Adressen oder Bestellungen. Die angeforderten Shopify-Berechtigungen sind `read_products`, `write_products` (Katalog und strukturierte Daten), `read_themes` (Prüfung, ob die Theme-Einbettung aktiv ist) und `write_pixels` (Aktivierung des oben genannten anonymen Traffic-Pixels).

## 3. Warum wir diese Daten verarbeiten und auf welcher Rechtsgrundlage

Wir verarbeiten diese Daten, um die Dienstleistung zu erbringen, für die Sie die App installiert haben — auf Grundlage von Art. 6 Abs. 1 lit. b DSGVO (Erfüllung eines Vertrags): Analyse und Verbesserung der Sichtbarkeit Ihres Katalogs auf generativen Suchmaschinen, einschließlich KI-gestützter FAQ-Entwürfe und Content-Rewriting, dem KI-Support-Chat in der App, dem wöchentlichen KI-Visibility-Tracking auf von Ihnen gewählten Prompts sowie der anonymen Messung des KI-Referral-Traffics — jeweils entweder vom Händler ausgelöst oder, beim Traffic-Pixel, an die Einwilligung in Ihrem Storefront gebunden.

## 4. Wie wir die Daten erfassen

Kontodaten werden einmalig über den OAuth-Ablauf von Shopify beim Installieren erfasst. Katalogdaten werden nur über die Admin-API von Shopify gelesen, wenn Sie eine Aktion vom Dashboard aus auslösen. Der Traffic-Pixel läuft auf Ihrem Storefront und meldet Ereignisse nur nach erfolgter Einwilligung; nichts anderes läuft im Hintergrund, ohne dass Sie es angefordert haben.

## 5. An wen wir die Daten weitergeben

- **Google Firebase / Cloud Firestore** — speichert Ihre Konfiguration, Sitzungen und Entwürfe. Google LLC (USA) nimmt am EU-US Data Privacy Framework teil. Die Daten werden in der Region europe-west1 (Belgien) gespeichert.
- **Anthropic PBC (USA)** — stellt das Claude-Modell bereit, das für FAQ-Entwürfe, Content-Rewriting und den KI-Support-Chat in der App verwendet wird, nur bei Ihrer ausdrücklichen Aktion. Erhält ausschließlich die von Ihnen bereitgestellten Produktattribute oder den Chat-Text — niemals Kundendaten.
- **OpenAI, Inc. (USA)** und **Perplexity AI, Inc. (USA)** — werden ausschließlich für das wöchentliche KI-Visibility-Tracking auf den Prompts verwendet, die Sie ausdrücklich zur Überwachung auswählen. Erhalten nur den Text der getrackten Prompts — niemals Kundendaten.
- **Google LLC (USA)** — stellt das Gemini-Modell bereit, das genauso wie OpenAI/Perplexity oben für das Visibility-Tracking verwendet wird (eine eigenständige Nutzung gegenüber Firebase/Firestore, das nur der Speicherung dient).
- **Resend, Inc. (USA)** — sendet uns eine Benachrichtigung mit dem Shop-Namen und dem Support-Chat-Transkript, nur wenn Sie im Support-Chat ausdrücklich bitten, mit einem Menschen zu sprechen.
- **Shopify Inc.** — die Plattform selbst und die Quelle der Admin-API und der Web-Pixel-Infrastruktur, die die App nutzt.

Wir verkaufen keine Daten und verwenden sie nicht für Marketing oder Verhaltensprofiling.

## 6. Wie lange wir die Daten aufbewahren

- **Sitzungstoken**: verwaltet durch den Offline-Token-Lebenszyklus von Shopify, automatisch rotiert.
- **Konfiguration, Audits, Entwürfe und Traffic-Ereignisse**: aufbewahrt, solange die App installiert ist. Eine Deinstallation löst den `shop/redact`-Webhook von Shopify aus, der die Konfiguration und Sitzungen Ihres Shops vollständig löscht.
- **Technische Protokolle**: aufbewahrt gemäß der Standard-Protokollierungsaufbewahrung von Google Cloud.

## 7. Ihre Rechte

Gemäß Art. 15–22 DSGVO können Sie Auskunft über Ihre Daten, die Berichtigung unrichtiger Daten oder die Löschung verlangen — am einfachsten durch Deinstallation der App — oder der Verarbeitung widersprechen. Sie können außerdem eine Beschwerde bei Ihrer zuständigen Datenschutzbehörde einreichen. Da die App niemals personenbezogene Daten von Endkunden verarbeitet, bestätigen die Compliance-Webhooks `customers/data_request` und `customers/redact`, dass nichts zu exportieren oder zu löschen ist.

## 8. Sicherheit

Der gesamte Datenverkehr läuft über HTTPS/TLS 1.2+. Shopify-Authentifizierungstoken werden dem Browser nie offengelegt. Jeder Webhook wird vor der Verarbeitung mit einer zeitkonstanten HMAC-SHA-256-Prüfung verifiziert. Die Datenbank ist ausschließlich über die eigene Serviceidentität des Backends der Hosting-Plattform erreichbar — es gibt keine statischen Zugangsdaten im Code, und direkter Client-Zugriff wird durch die eigenen Sicherheitsregeln der Datenbank verweigert. Daten werden verschlüsselt gespeichert und übertragen.

## 9. Änderungen

Wir können diese Richtlinie von Zeit zu Zeit aktualisieren. Wesentliche Änderungen werden hier abgebildet, das Datum oben wird stets aktuell gehalten.

---

**Fragen zu Ihren Daten?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Zurück zum Hilfe-Center](index.html)
