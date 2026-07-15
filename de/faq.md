---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
lang: de
---

# Häufig gestellte Fragen

<div class="lang-switcher">
{% include lang-switcher.html current="de" slug="faq" %}
</div>

**Was ist der Unterschied zwischen GEO und SEO?**
Klassisches SEO optimiert für Suchmaschinen, die Links ranken und auflisten. GEO (Generative Engine Optimization) optimiert für KI-Systeme, die Ihre Inhalte lesen und direkt eine Antwort oder Empfehlung generieren — ChatGPT, Perplexity, Gemini, Claude und Google AI Overviews. Beide überschneiden sich, aber GEO berücksichtigt Dinge, die klassische SEO-Tools nicht prüfen: ob Ihre Produktseite vollständige strukturierte Daten enthält, ob ein KI-Crawler Ihre Inhalte tatsächlich ohne JavaScript-Ausführung lesen kann, und ob Ihr Text so geschrieben ist, dass er sich leicht zitieren lässt.

**Greift die App jemals auf Kundendaten zu?**
Nein, keine personenbezogenen Kundendaten. Die Shopify-Berechtigungen der App sind `read_products`, `write_products`, `read_themes` und `write_pixels` — zum Lesen und Verbessern Ihres Katalogs, zur Prüfung, ob die Theme-Einbettung aktiv ist, und zur Aktivierung eines anonymen Storefront-Traffic-Pixels (siehe unten). Sie fordert nie Bestellungen oder Kundendatensätze an. Die vollständige Übersicht finden Sie in der [Datenschutzerklärung](privacy.html).

**Was ist der KI-Referral-Traffic-Pixel, und verfolgt er meine Kunden?**
Bei Grow und Unlimited erkennt ein kleiner Web Pixel, wenn ein Storefront-Besuch von einer bekannten KI-Engine stammt (über den Browser-Referrer), und meldet die Engine, die Seite und einen Zeitstempel — nichts, was den Besucher identifiziert, keine Cookies, keine Sitzungsdaten. Er läuft nur, wenn der Besucher bereits über den Cookie-Banner Ihres Shops der Analyse zugestimmt hat (Shopifys Customer Privacy API). Er wird für eine Dashboard-Kachel genutzt („KI-Referral-Traffic, letzte 7 Tage") — das Gegenstück zum Visibility-AI-Tracking, das Ihnen zeigt, ob Sie erwähnt werden, aber nicht, ob diese Erwähnung jemanden geschickt hat.

**Was ändert die Schaltfläche „Beheben" beim Katalog-Audit tatsächlich?**
Sie schreibt fehlende schema.org-Strukturdaten in ein Produkt-Metafeld — etwa technische Spezifikationen, die aus Ihren vorhandenen Produktoptionen abgeleitet werden. Sie ändert nie Produkttitel, Beschreibung, Bilder oder Preis, und sie erfindet nie Daten, die sie nicht verifizieren kann: Ein fehlender Barcode zum Beispiel bleibt fehlend, statt geraten zu werden.

**Sind die FAQ-Antworten und umgeschriebenen Beschreibungen von der KI erfunden, oder basieren sie auf meinem tatsächlichen Produkt?**
Das Modell sieht ausschließlich die bereits vorhandenen Produktdaten — Titel, Beschreibung, Hersteller und technische Spezifikationen — und wird ausdrücklich angewiesen, nichts hinzuzufügen, was nicht in diesen Daten enthalten ist. Sie prüfen jede FAQ oder umgeschriebene Beschreibung, bevor sie veröffentlicht wird; nichts geht automatisch live.

**Was passiert mit meinen Daten, wenn ich die App deinstalliere?**
Ihre Shop-Konfiguration, gespeicherte Audits, FAQ- und Content-Rewrite-Entwürfe, Visibility-Prompts und KI-Referral-Traffic-Ereignisse werden automatisch gelöscht, sobald Shopify uns über die Deinstallation benachrichtigt. Die App behält nichts, nachdem Sie sie verlassen haben.

**Kann ich ohne Kontakt zum Support kündigen oder herabstufen?**
Ja. Gehen Sie in der App jederzeit zu **Preise** und wechseln Sie zu Free — die Änderung wirkt sofort, keine E-Mail erforderlich.

## Plan-Limits

| Funktion | Free | Grow | Unlimited |
|---|---|---|---|
| Katalog-Audit | Erste 20 Produkte, einmalig, kein Verlauf | Vollständiger Katalog + Verlauf | Vollständiger Katalog + Verlauf |
| Crawler-Simulator | 20/Monat | 300/Monat | 1.000/Monat |
| Wettbewerbsvergleich | 10/Monat | 50/Monat | 150/Monat |
| FAQ-Generierung | Nicht enthalten | 500/Monat | 500/Monat |
| Content-Rewrite | Nicht enthalten | 300/Monat | 300/Monat |
| Visibility AI (getrackte Prompts) | Nicht enthalten | 5 Prompts | 15 Prompts |
| KI-Referral-Traffic-Pixel | Nicht enthalten | Enthalten | Enthalten |
| KI-Support-Chat | 1.000 Nachrichten/Monat | 1.000 Nachrichten/Monat | 1.000 Nachrichten/Monat |
| Oberflächensprachen | Alle 30 | Alle 30 | Alle 30 |

Monatliche Preise: Free $0, Grow $9.99, Unlimited $19.99. Bei jährlicher Abrechnung sind Grow/Unlimited im Vergleich zur monatlichen Zahlung ungefähr zwei Monate gratis.

**Warum deckt der Free-Plan nur 20 Produkte ab?**
So können Sie echte Ergebnisse an Ihrem eigenen Katalog sehen, bevor Sie sich für einen kostenpflichtigen Plan entscheiden. Grow und Unlimited entfernen diese Obergrenze und speichern den vollständigen Verlauf früherer Audits.

**Gibt es wirklich eine Obergrenze für die FAQ-Generierung, sogar bei Unlimited?**
Ja — 500 Generierungen pro Monat, ganz bewusst, sogar im höchsten Plan. Das hält die Funktion beim aktuellen Preis nachhaltig; wenn Sie einen sehr großen Katalog haben und mehr benötigen, kontaktieren Sie uns, und wir finden eine Lösung.

**Warum ist der KI-Support-Chat auf jedem Plan gleich?**
Das ist eine Produktentscheidung, kein Versehen: Support ist für alle enthalten, nie ein kostenpflichtiges Unterscheidungsmerkmal. Das Nachrichtenlimit (1.000/Monat) existiert nur als technische Absicherung gegen Missbrauch, nicht als reales Limit — keine legitime Nutzung kommt auch nur in die Nähe davon.

**Ich habe einen Fehler gefunden oder etwas sieht falsch aus. Wem sage ich das?**
Schreiben Sie an [info@ifgecommerce.com](mailto:info@ifgecommerce.com) mit einer Beschreibung dessen, was Sie gesehen haben, und wenn möglich, welches Produkt oder welche Seite betroffen ist — das reicht meist aus, um die Ursache schnell zu finden. Sie können auch den KI-Support-Chat in der App nutzen und darum bitten, mit einem Menschen zu sprechen.

[← Zurück zum Hilfe-Center](index.html)
