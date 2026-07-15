---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
lang: fr
---

# Journal des modifications

<div class="lang-switcher">
{% include lang-switcher.html current="fr" slug="changelog" pages="en,it,de,fr,es" %}
</div>

Tous les changements qui atteignent les marchands, du plus récent au plus ancien. Il s'agit d'une documentation technique, maintenue dans 5 langues (anglais, italien, allemand, français, espagnol) plutôt que dans les 30 langues prises en charge par le reste du Centre d'aide.

## Juillet 2026

**Suivi du trafic de référencement IA** — Ajout d'un Web Pixel (Grow/Unlimited) qui détecte les visites de la boutique en ligne arrivant depuis un moteur IA reconnu (ChatGPT, Perplexity, Claude, Gemini, Copilot) et les signale sur une nouvelle tuile du tableau de bord, conditionnée au consentement et entièrement anonyme — le pendant du suivi Visibility AI : pas seulement « sommes-nous mentionnés », mais « cette mention envoie-t-elle quelqu'un ».

**Améliorations du tableau de bord et de la navigation** — Ajout d'un véritable état vide pour la première utilisation, d'un squelette de chargement pendant la navigation entre les pages, et d'une répartition par bot sur la page crawler indiquant si une règle `robots.txt` a été trouvée nommément ou héritée du groupe générique.

**Refonte de l'onboarding** — La barre de progression de l'assistant de configuration est devenue une liste de contrôle étape par étape, avec une bannière de confirmation visible à la fin au lieu d'un rechargement instantané et non confirmé.

**Facturation et e-mail d'assistance** — Le contact d'assistance et de confidentialité a été déplacé vers `info@ifgecommerce.com`.

**Internal Link & Entity Graph Coach** — Nouvelle analyse de la façon dont les produits se connectent entre eux via des collections, marques et tags communs, avec des suggestions explicables et un résumé sur le tableau de bord.

**Readiness Matrix** — Le tableau de bord dispose désormais d'un panneau unique, visible en un coup d'œil, agrégeant chaque signal GEO suivi par l'application : extractibilité du contenu, schéma Organization, `llms.txt`, `agents.md`, accès des crawlers, préparation MCP, connectivité Link Coach et (une fois déployé) trafic de référencement IA.

**Moteur de réécriture de contenu** — Ajout d'un outil assisté par IA pour réécrire une description de produit afin qu'elle soit plus dense en faits vérifiables et plus facile à citer pour un moteur génératif, avec une relecture avant/après obligatoire avant toute réécriture.

**Comparaison avec la concurrence** — Collez l'URL de la page produit d'un concurrent et visualisez les mêmes signaux GEO comparés côte à côte avec votre propre produit.

**Suivi Visibility AI** — Vérifications hebdomadaires automatisées pour savoir si Claude, ChatGPT, Gemini et Perplexity mentionnent votre boutique sur les questions que vous choisissez de surveiller, avec un graphique de tendance et une répartition par moteur.

**Schéma Organization et `agents.md`** — Ajout de données structurées d'identité d'entreprise (raison sociale, numéro de TVA/identifiant fiscal, adresse) pour les systèmes IA qui vérifient qu'une entreprise est réelle, et d'un fichier `agents.md` généré décrivant la boutique aux agents d'achat autonomes.

**Facturation** — Les marchands peuvent s'abonner à Grow ou Unlimited, mensuellement ou annuellement, directement depuis la page Tarifs, et revenir à l'offre Free à tout moment sans contacter l'assistance.

**Politique de confidentialité et revue de conformité App Store** — Publication de ce Centre d'aide et d'une politique de confidentialité formelle ; vérification que les permissions Shopify de l'application et la gestion des webhooks RGPD répondent aux exigences de l'App Store avant la soumission.

**Génération de FAQ assistée par IA** — Génération de trois à cinq paires question-réponse par produit à partir de son titre, sa description et ses spécifications existants, relecture, puis publication de celles que vous approuvez. Les FAQ publiées apparaissent sur la page produit et en tant que données structurées `FAQPage`.

**Score d'extractibilité du contenu (chunking)** — L'audit du catalogue évalue désormais aussi la facilité avec laquelle un système IA peut extraire et citer la description de chaque produit — pas seulement la présence des champs de données structurées, mais l'utilisabilité de la rédaction elle-même.

**Simulateur de crawler** — Récupérez n'importe quelle page produit exactement comme la voit un crawler IA — sans JavaScript, comme GPTBot, ClaudeBot et PerplexityBot — y compris des vérifications `robots.txt` par bot.

**Audit du catalogue et corrections en un clic** — Lancement de l'audit principal : analyse votre catalogue sur neuf champs de données structurées, note chaque produit, et corrige ce qu'il peut faire de manière fiable en un clic. Ajout également d'une véritable génération de `llms.txt`, servie à la racine réelle de votre boutique.

## Antérieurement

Version initiale : configuration de l'application intégrée, authentification Shopify, et infrastructure de données sous-jacente.

[← Retour au Centre d'aide](index.html)
