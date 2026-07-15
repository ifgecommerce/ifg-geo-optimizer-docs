---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
lang: de
---

# Erste Schritte

<div class="lang-switcher">
{% include lang-switcher.html current="de" slug="getting-started" %}
</div>

IFG GEO Optimizer hat neun Bereiche, die nach Abschluss der Einrichtung alle über die obere Navigation erreichbar sind: **Dashboard**, **Katalog-Audit**, **Crawler KI**, **Produkt-FAQ**, **Link Coach**, **Visibility AI**, **Preise**, **Einstellungen** und **Support**. Diese Anleitung führt durch alle, in der Reihenfolge, in der die meisten Händler sie nutzen.

## 1. Installieren und den Einrichtungsassistenten abschließen

Beim ersten Öffnen sammelt eine kurze geführte Einrichtung (etwa 2 Minuten) die Grundlagen: Oberflächensprache, die Details Ihrer Rückgabe- und Versandrichtlinie, Ihre Unternehmensdaten und — der Schritt, der technisch wirklich zählt — die Aktivierung der App-Einbettung **GEO Schema** im Theme-Editor. Nichts, was die App danach tut, erreicht Ihren Storefront, bevor diese Einbettung aktiviert ist — es lohnt sich also, diesen Schritt nicht zu überspringen. Sie können jede dieser Angaben später jederzeit in **Einstellungen** ändern.

## 2. Dashboard

Ihre Zentrale. Sie zeigt Ihren aktuellen GEO-Score (aus Ihrem letzten Audit), eine **Readiness Matrix** mit acht Signalen auf einen Blick — Content-Extrahierbarkeit, Organization-Schema, `llms.txt`, `agents.md`, Crawler-Zugriff, MCP-Bereitschaft, Link-Coach-Konnektivität und KI-Referral-Traffic —, dazu eine priorisierte „Das zuerst beheben"-Liste und die Nutzungszähler Ihres Plans (FAQ-Generierungen, Katalogumfang). Von hier aus führt alles direkt zu der Seite, auf der Sie handeln können.

## 3. Katalog-Audit

Klicken Sie auf **Katalog erneut scannen**, um jedes Produkt anhand von neun strukturierten Datenfeldern zu prüfen, nach denen Suchmaschinen suchen: Bild, Beschreibung, Marke, SKU, GTIN, Preis, technische Spezifikationen, Rückgaberichtlinie und Versandrichtlinie. Produkte unter 80/100 zeigen genau, was fehlt.

- **Ein-Klick-Korrektur**: Wo die App die fehlenden Daten sicher ableiten kann (meist technische Spezifikationen aus Ihren vorhandenen Produktoptionen), sehen Sie eine Schaltfläche **Beheben**, die sie direkt in die strukturierten Daten des Produkts schreibt. Bei Feldern, die die App nicht verifizieren kann, wird nichts geraten — ein fehlender Barcode zum Beispiel bleibt fehlend, statt erfunden zu werden.
- **Content-Chunking-Score**: Neben der Prüfung der strukturierten Daten erhält jedes Produkt einen eigenen Extrahierbarkeits-Score — nicht „ist das Feld vorhanden", sondern „kann ein KI-/RAG-System aus dieser Beschreibung tatsächlich einen sauberen Fakt herausziehen". Dünner, adjektivlastiger Text erhält eine niedrigere Bewertung, selbst bei perfektem schema.org-Markup.
- **`llms.txt`**: erzeugt eine echte, standardkonforme `llms.txt`-Datei, die Ihren Katalog für KI-Systeme zusammenfasst und an der tatsächlichen Root Ihres Shops (`/llms.txt`) ausgeliefert wird — nicht versteckt unter einem App-Proxy-Pfad, wo Crawler sie nicht finden.
- **`agents.md`**: erzeugt eine Datei, die Ihren Shop für autonome Shopping-Agenten beschreibt — Varianten, Suche, Checkout — ausschließlich aus echten Daten, die Ihr Shop bereits offenlegt, nichts erfunden.
- **Organization-Schema**: veröffentlicht Ihre Unternehmensdaten (Rechtsform, USt-IdNr./Steuernummer, Adresse) als strukturierte Daten, damit KI-Engines prüfen können, dass Sie ein echtes, verantwortliches Unternehmen sind, bevor sie Sie empfehlen.

Im Free-Plan deckt der Audit Ihre ersten 20 Produkte ab, einmalig, ohne gespeicherten Verlauf. Grow und Unlimited scannen Ihren gesamten Katalog und behalten jeden vergangenen Scan für Trendvergleiche.

## 4. Crawler KI

Wählen Sie ein Produkt aus, und die App ruft dessen Seite genau so ab, wie es ein KI-Crawler tut — ohne JavaScript-Ausführung, genau wie GPTBot, ClaudeBot oder PerplexityBot —, sodass Sie exakt sehen, was für diese Engines sichtbar ist: ob Ihre `robots.txt` sie blockiert (pro Bot geprüft, nicht nur ein generisches Erlauben/Verbieten) und ob Ihre strukturierten Daten im rohen HTML, das diese Bots lesen, tatsächlich erhalten bleiben.

**Wettbewerbsvergleich** (eigener Tab auf dieser Seite): Fügen Sie die Produkt-URL eines Wettbewerbers ein und erhalten Sie dieselben GEO-Signale, direkt neben Ihren eigenen verglichen — derselbe Unterschied, den Sie aus einem manuellen Audit erhalten würden, ohne sich bei den Tools des Wettbewerbers anmelden zu müssen.

## 5. Produkt-FAQ

Bei Grow oder Unlimited wählen Sie ein Produkt aus und klicken auf **FAQs generieren**, um drei bis fünf Frage-Antwort-Paare zu erhalten, die ausschließlich aus dem tatsächlichen Titel, der Beschreibung, dem Hersteller und den Spezifikationen dieses Produkts entworfen werden — das Modell wird ausdrücklich angewiesen, nie ein Detail hinzuzufügen, das nicht bereits in Ihren Daten steht. Prüfen Sie jeden Entwurf; nichts wird veröffentlicht ohne Ihre ausdrückliche **Freigabe**. Freigegebene FAQs erscheinen auf der Live-Produktseite und werden als `FAQPage`-Strukturdaten markiert — so sind sie sowohl für Menschen lesbar als auch maschinell zitierbar.

**Content-Rewrite** (eigener Tab auf dieser Seite): Die App kann eine Produktbeschreibung so umschreiben, dass sie dichter an verifizierbaren Fakten und leichter für eine generative Engine zu zitieren ist — Sie sehen immer einen Vorher-Nachher-Vergleich und geben ihn frei, bevor irgendetwas in das Produkt zurückgeschrieben wird.

## 6. Link Coach

Analysiert, wie gut Ihre Produkte über gemeinsame Kollektionen, Hersteller und Tags miteinander verbunden sind — interne Verlinkung ist ein Signal, das KI-Systeme nutzen, um zu verstehen, was Ihr Katalog insgesamt abdeckt, nicht nur eine einzelne Seite. Zeigt verwaiste Produkte ohne aussagekräftige Verbindungen sowie erklärbare Vorschläge, um das zu beheben.

## 7. Visibility AI

Fügen Sie eine Handvoll Prompts hinzu, die ein Kunde realistisch an einen KI-Assistenten stellen könnte (das Limit hängt von Ihrem Plan ab — siehe Preise unten), und jede Woche prüft die App, ob Claude, ChatGPT, Gemini und Perplexity Ihren Shop in der Antwort erwähnen, im Zeitverlauf pro Engine nachverfolgt. Bei Grow und Unlimited zeigt dies zusätzlich, wie Sie im Vergleich zu benannten Wettbewerbern bei denselben Prompts abschneiden.

**KI-Referral-Traffic** (Grow und Unlimited): Ein leichtgewichtiger, datenschutzfreundlicher Pixel erkennt, wenn ein Storefront-Besuch tatsächlich von einer dieser KI-Engines stammt (über den Referrer, nur nachdem der Besucher über den Cookie-Banner Ihres Shops der Analyse zugestimmt hat) und meldet, wie viele solcher Besuche Sie in den letzten 7 Tagen hatten — die zweite Hälfte des Kreislaufs, die das Visibility-Tracking allein nicht zeigen kann: nicht nur „werden wir erwähnt", sondern „schickt diese Erwähnung auch jemanden".

## 8. Support

Ein KI-Chat-Assistent lebt in der App (Symbol unten rechts) für Fragen zu GEO, Ihren Audit-Ergebnissen oder wie eine bestimmte Funktion funktioniert. Wenn er nicht weiterhelfen kann, können Sie darum bitten, mit einem Menschen zu sprechen, und das Gespräch wird direkt an IFG eCommerce weitergeleitet.

## 9. Einstellungen

Hier verwalten Sie die Antworten aus dem Einrichtungsassistenten (Richtlinien, Unternehmensdaten, Oberflächensprache — sofortiger Wechsel zwischen 30 Sprachen, ohne Ladeverzögerung), prüfen erneut die Aktivierung der Theme-Einbettung und sehen die Shopify-Berechtigungen Ihres Kontos.

## 10. Preise

**Preise** zeigt Free, Grow und Unlimited im Vergleich, monatlich oder jährlich (jährlich sind bei beiden kostenpflichtigen Stufen ungefähr 2 Monate gratis). Sie können jederzeit direkt in der App upgraden, downgraden oder zu Free zurückkehren — kein E-Mail-Kontakt nötig. Die genauen Plan-Limits finden Sie in den [FAQ](faq.html).

Das ist der komplette Ablauf. Die meisten Händler führen nach dem Hinzufügen neuer Produkte erneut einen Audit durch, prüfen den Crawler-Simulator, sobald sie eine Beschreibung aktualisieren, und werfen wöchentlich einen Blick auf die Readiness Matrix im Dashboard.

[← Zurück zum Hilfe-Center](index.html)
