---
title: IFG GEO Optimizer
description: Dokumentation, FAQ und rechtliche Seiten für die Shopify-App IFG GEO Optimizer.
lang: de
---

# Changelog

<div class="lang-switcher">
{% include lang-switcher.html current="de" slug="changelog" pages="en,it,de,fr,es" %}
</div>

Alle Änderungen, die bei Händlern ankommen, neueste zuerst. Dies ist technische Dokumentation, die nur in 5 Sprachen gepflegt wird (Englisch, Italienisch, Deutsch, Französisch, Spanisch), nicht in allen 30 Sprachen, die der Rest des Hilfe-Centers unterstützt.

## Juli 2026

**KI-Referral-Traffic-Tracking** — Einen Web Pixel (Grow/Unlimited) hinzugefügt, der Storefront-Besuche erkennt, die von einer bekannten KI-Engine stammen (ChatGPT, Perplexity, Claude, Gemini, Copilot), und diese auf einer neuen Dashboard-Kachel meldet, einwilligungsgebunden und vollständig anonym — das Gegenstück zum Visibility-AI-Tracking: nicht nur „werden wir erwähnt", sondern „schickt diese Erwähnung auch jemanden".

**Feinschliff bei Dashboard und Navigation** — Einen ordentlichen Leerzustand für die Erstnutzung, ein Lade-Skelett während der Seitennavigation und eine Bot-für-Bot-Aufschlüsselung auf der Crawler-Seite hinzugefügt, die zeigt, ob eine `robots.txt`-Regel namentlich getroffen oder von der Wildcard-Gruppe geerbt wurde.

**Neugestaltung des Onboardings** — Der Fortschrittsbalken des Einrichtungsassistenten wurde zu einer schrittweisen Checkliste, mit einem sichtbaren Bestätigungsbanner am Ende, statt eines sofortigen, unbestätigten Neuladens.

**Abrechnung und Support-E-Mail** — Support- und Datenschutzkontakt zu `info@ifgecommerce.com` verschoben.

**Internal Link & Entity Graph Coach** — Neue Analyse, wie gut Produkte über gemeinsame Kollektionen, Hersteller und Tags miteinander verbunden sind, mit erklärbaren Vorschlägen und einer Dashboard-Zusammenfassung.

**Readiness Matrix** — Das Dashboard erhielt ein einziges, auf einen Blick erfassbares Panel, das jedes von der App verfolgte GEO-Signal zusammenfasst: Content-Extrahierbarkeit, Organization-Schema, `llms.txt`, `agents.md`, Crawler-Zugriff, MCP-Bereitschaft, Link-Coach-Konnektivität und (sobald verfügbar) KI-Referral-Traffic.

**Content-Rewrite-Engine** — Ein KI-gestütztes Tool hinzugefügt, um eine Produktbeschreibung so umzuschreiben, dass sie dichter an verifizierbaren Fakten und leichter für eine generative Engine zu zitieren ist, mit einer verpflichtenden Vorher-Nachher-Prüfung, bevor irgendetwas zurückgeschrieben wird.

**Wettbewerbsvergleich** — Fügen Sie die Produkt-URL eines Wettbewerbers ein und sehen Sie dieselben GEO-Signale, direkt neben Ihrem eigenen Produkt verglichen.

**Visibility-AI-Tracking** — Wöchentliche automatisierte Prüfungen, ob Claude, ChatGPT, Gemini und Perplexity Ihren Shop bei von Ihnen gewählten Prompts erwähnen, mit einem Trenddiagramm und einer Aufschlüsselung pro Engine.

**Organization-Schema und `agents.md`** — Strukturierte Unternehmensidentitätsdaten hinzugefügt (Rechtsform, USt-IdNr./Steuernummer, Adresse) für KI-Systeme, die prüfen, ob ein Unternehmen real ist, sowie eine generierte `agents.md`-Datei, die den Shop für autonome Shopping-Agenten beschreibt.

**Abrechnung** — Händler können ab sofort direkt über die Seite „Preise" Grow oder Unlimited abonnieren, monatlich oder jährlich, und jederzeit ohne Kontakt zum Support wieder zu Free zurückkehren.

**Datenschutzerklärung und Prüfung der App-Store-Konformität** — Dieses Hilfe-Center und eine formelle Datenschutzerklärung veröffentlicht; bestätigt, dass die Shopify-Berechtigungen der App und die Behandlung der DSGVO-Webhooks den Anforderungen des App Store vor der Einreichung entsprechen.

**KI-gestützte FAQ-Generierung** — Generieren Sie drei bis fünf Frage-Antwort-Paare pro Produkt aus dessen vorhandenem Titel, Beschreibung und Spezifikationen, prüfen Sie sie und veröffentlichen Sie die freigegebenen. Veröffentlichte FAQs erscheinen auf der Produktseite und als `FAQPage`-Strukturdaten.

**Content-Extrahierbarkeit (Chunking-Score)** — Der Katalog-Audit bewertet nun auch, wie leicht die Beschreibung jedes Produkts für ein KI-System zu extrahieren und zu zitieren ist — nicht nur, ob strukturierte Datenfelder vorhanden sind, sondern ob der Text selbst nutzbar ist.

**Crawler-Simulator** — Rufen Sie jede Produktseite genau so ab, wie sie ein KI-Crawler sieht — ohne JavaScript, genau wie GPTBot, ClaudeBot und PerplexityBot — einschließlich Prüfungen der `robots.txt` pro Bot.

**Katalog-Audit und Ein-Klick-Korrekturen** — Den zentralen Audit eingeführt: scannt Ihren Katalog anhand von neun strukturierten Datenfeldern, bewertet jedes Produkt und behebt, was sicher automatisch behoben werden kann, mit einem Klick. Außerdem echte `llms.txt`-Generierung hinzugefügt, ausgeliefert an der tatsächlichen Root Ihres Shops.

## Früher

Erstveröffentlichung: Einrichtung der eingebetteten App, Shopify-Authentifizierung und die zugrunde liegende Dateninfrastruktur.

[← Zurück zum Hilfe-Center](index.html)
