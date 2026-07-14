---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
---

# Erste Schritte

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <span class="lang-item lang-current"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</span>
  <a class="lang-item" href="../fr/"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</a>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

Dieser Leitfaden führt Sie durch alles, von der Installation der App bis zur Veröffentlichung Ihrer ersten KI-optimierten FAQ.

## 1. App installieren und Dashboard öffnen

Nach der Installation öffnet sich IFG GEO Optimizer direkt in Ihrem Shopify-Admin. Das Dashboard ist Ihre Zentrale — es füllt sich mit dem GEO-Score Ihres Shops und den letzten Aktivitäten, sobald Sie die App nutzen.

## 2. Ihre Richtlinien hinterlegen

Gehen Sie zu **Einstellungen** und tragen Sie die Details Ihrer Rückgabe- und Versandrichtlinie ein (Rückgabefrist, wer die Rücksendekosten trägt, Bearbeitungs- und Versandzeiten, Zielland). Diese Angaben fließen direkt in die strukturierten Daten ein, die die App für jedes Produkt veröffentlicht — Shopifys Produktseiten geben diese Informationen sonst nicht an Suchmaschinen weiter, daher verbessert allein dieser Schritt Ihren Audit-Score messbar.

## 3. Ihren ersten Katalog-Audit durchführen

Öffnen Sie **Katalog-Audit** und klicken Sie auf **Katalog erneut scannen**. Die App liest Ihren Produktkatalog über die Admin-API von Shopify und prüft jedes Produkt anhand von neun strukturierten Datenfeldern, nach denen Suchmaschinen suchen: Bild, Beschreibung, Marke, SKU, GTIN, Preis, technische Spezifikationen, Rückgaberichtlinie und Versandrichtlinie.

Produkte unter 80/100 zeigen genau, was fehlt. Wo die App das automatisch beheben kann — meist indem sie technische Spezifikationen aus Ihren vorhandenen Produktoptionen ableitet — sehen Sie eine Schaltfläche **Beheben**. Ein Klick schreibt die fehlenden schema.org-Daten direkt in das Produkt; nichts wird geraten oder erfunden bei Feldern, die die App nicht sicher ableiten kann (ein Barcode zum Beispiel wird nie automatisch generiert).

Im Free-Plan deckt der Audit Ihre ersten 20 Produkte ab und speichert keinen Verlauf. Grow und Unlimited decken Ihren gesamten Katalog ab und speichern jeden Scan.

## 4. Den Theme-Block aktivieren

Die durch den Audit korrigierten strukturierten Daten erscheinen erst in Ihrem Storefront, wenn Sie sie aktivieren. Gehen Sie in Ihrem Theme-Editor zu **App-Einbettungen** und schalten Sie **GEO Schema** ein. Das ist eine einmalige Aktivierung — danach enthält jede Produktseite automatisch das von Ihrem Audit generierte JSON-LD.

## 5. Prüfen, was ein Bot tatsächlich sieht

Öffnen Sie **Crawler-KI** und wählen Sie ein Produkt aus. Die App ruft die Seite genau so ab, wie es ein KI-Crawler tut — ohne JavaScript-Ausführung, genau wie GPTBot, ClaudeBot oder PerplexityBot — sodass Sie exakt sehen können, was für diese Systeme sichtbar ist, einschließlich ob Ihre robots.txt sie blockiert und ob Ihre strukturierten Daten im rohen HTML vollständig sind.

## 6. FAQs generieren

Bei Grow oder Unlimited öffnen Sie **Produkt-FAQ**, wählen ein Produkt aus und klicken auf **3 FAQs generieren**. Die App erstellt drei Frage-Antwort-Paare aus dem tatsächlichen Titel, der Beschreibung und den Spezifikationen Ihres Produkts — nie erfundene Details. Prüfen Sie jeden Entwurf und klicken Sie dann auf **Freigeben & veröffentlichen** für die, die live gehen sollen; freigegebene FAQs erscheinen auf der Produktseite und werden als FAQPage-Strukturdaten für Suchmaschinen markiert. Nichts wird ohne Ihre Prüfung veröffentlicht.

## 7. Einen Plan wählen

**Preise** zeigt Free, Grow und Unlimited im Vergleich, mit monatlicher und jährlicher Abrechnung. Sie können jederzeit direkt in der App den Plan wechseln oder zu Free zurückkehren — kein Kontakt zum Support nötig, um herabzustufen.

Das ist der komplette Ablauf. Die meisten Händler führen nach dem Hinzufügen neuer Produkte erneut einen Audit durch und prüfen den Crawler-Simulator, sobald sie eine Produktbeschreibung aktualisieren.

[← Zurück zum Hilfe-Center](index.html)
