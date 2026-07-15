---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
lang: fr
---

# Prise en main

<div class="lang-switcher">
{% include lang-switcher.html current="fr" slug="getting-started" %}
</div>

IFG GEO Optimizer comprend neuf sections, toutes accessibles depuis la navigation supérieure une fois la configuration terminée : **Tableau de bord**, **Audit du catalogue**, **Crawler IA**, **FAQ produit**, **Link Coach**, **Visibility AI**, **Tarifs**, **Paramètres** et **Assistance**. Ce guide les présente toutes, dans l'ordre dans lequel la plupart des marchands les utilisent.

## 1. Installer et terminer l'assistant de configuration

À la première ouverture, une courte configuration guidée (environ 2 minutes) recueille les informations essentielles : la langue de l'interface, les détails de votre politique de retour et d'expédition, les informations de votre entreprise et — la seule étape qui compte vraiment sur le plan technique — l'activation du bloc d'application **GEO Schema** dans l'éditeur de thème. Rien de ce que fait l'application ensuite n'atteint votre boutique en ligne tant que ce bloc n'est pas activé, mieux vaut donc ne pas sauter cette étape. Vous pouvez toujours modifier ces réponses plus tard depuis **Paramètres**.

## 2. Tableau de bord

Votre point de départ. Il affiche votre score GEO actuel (basé sur votre dernier audit), une **Readiness Matrix** avec huit signaux visibles en un coup d'œil — extractibilité du contenu, schéma Organization, `llms.txt`, `agents.md`, accès des crawlers, préparation MCP, connectivité Link Coach et trafic de référencement IA — ainsi qu'une liste priorisée « à corriger en premier » et les compteurs d'utilisation de votre offre (générations de FAQ, taille du catalogue). Tout ici renvoie directement vers la page où vous pouvez agir.

## 3. Audit du catalogue

Cliquez sur **Réanalyser le catalogue** pour vérifier chaque produit sur neuf champs de données structurées recherchés par les moteurs de recherche : image, description, marque, référence (SKU), GTIN, prix, spécifications techniques, politique de retour et politique d'expédition. Les produits en dessous de 80/100 montrent exactement ce qui manque.

- **Correction en un clic** : lorsque l'application peut dériver les données manquantes en toute sécurité (généralement les spécifications techniques à partir de vos options de produit existantes), un bouton **Corriger** apparaît et écrit les données directement dans les données structurées du produit. Rien n'est deviné pour les champs que l'application ne peut pas vérifier — un code-barres manquant, par exemple, reste manquant plutôt que d'être inventé.
- **Score de chunking du contenu** : en plus de la vérification des données structurées, chaque produit reçoit un score d'extractibilité distinct — pas « le champ est-il présent » mais « un système IA/RAG peut-il réellement extraire un fait précis de cette description ». Un texte pauvre et truffé d'adjectifs obtient un score plus bas, même avec un balisage schema.org parfait.
- **`llms.txt`** : génère un véritable fichier `llms.txt` conforme aux standards, résumant votre catalogue pour les systèmes d'IA, servi à la racine réelle de votre boutique (`/llms.txt`), et non enfoui sous un chemin de proxy d'application où les crawlers ne le trouveraient pas.
- **`agents.md`** : génère un fichier décrivant votre boutique aux agents d'achat autonomes — variantes, recherche, paiement — construit uniquement à partir de données réelles déjà exposées par votre boutique, rien n'est inventé.
- **Schéma Organization** : publie les informations de votre entreprise (raison sociale, numéro de TVA/identifiant fiscal, adresse) sous forme de données structurées, afin que les moteurs IA puissent vérifier que vous êtes une entreprise réelle et identifiable avant de vous recommander.

Sur l'offre Free, les audits couvrent vos 20 premiers produits, une seule fois, sans historique conservé. Grow et Unlimited analysent tout votre catalogue et conservent chaque analyse passée pour comparer les tendances.

## 4. Crawler IA

Choisissez un produit et l'application récupère sa page exactement comme le ferait un crawler IA — sans exécution JavaScript, comme GPTBot, ClaudeBot ou PerplexityBot — afin que vous voyiez précisément ce qui est visible pour ces moteurs : si votre `robots.txt` les bloque (vérifié bot par bot, pas seulement une autorisation/interdiction générique), et si vos données structurées survivent réellement dans le HTML brut que ces bots lisent.

**Comparaison avec la concurrence** (dans son propre onglet sur cette page) : collez l'URL de la page produit d'un concurrent et obtenez les mêmes signaux GEO comparés côte à côte avec les vôtres — le même type d'écart que vous obtiendriez avec un audit manuel, sans avoir besoin de vous inscrire aux outils du concurrent.

## 5. FAQ produit

Sur Grow ou Unlimited, choisissez un produit et cliquez sur **Générer les FAQ** pour obtenir de trois à cinq paires question-réponse rédigées uniquement à partir du titre, de la description, de la marque et des spécifications réels de ce produit — le modèle reçoit l'instruction explicite de ne jamais ajouter un détail absent de vos données. Relisez chaque brouillon ; rien n'est publié sans votre **Approbation** explicite. Les FAQ approuvées apparaissent sur la page produit en ligne et sont balisées en données structurées `FAQPage`, ce qui les rend à la fois lisibles par les humains et citables par les machines.

**Réécriture de contenu** (dans son propre onglet sur cette page) : l'application peut réécrire une description de produit pour la rendre plus dense en faits vérifiables et plus facile à citer pour un moteur génératif — vous voyez toujours une comparaison avant/après et devez approuver avant que quoi que ce soit ne soit réécrit sur le produit.

## 6. Link Coach

Analyse la façon dont vos produits sont reliés entre eux via des collections, marques et tags communs — le maillage interne est un signal que les systèmes d'IA utilisent pour comprendre ce que couvre votre catalogue dans son ensemble, pas seulement page par page. Affiche les produits orphelins sans connexions significatives et des suggestions explicables pour y remédier.

## 7. Visibility AI

Ajoutez jusqu'à quelques questions qu'un client pourrait réalistiquement poser à un assistant IA (la limite dépend de votre offre — voir Tarifs ci-dessous), et chaque semaine l'application vérifie si Claude, ChatGPT, Gemini et Perplexity mentionnent votre boutique dans la réponse, suivi dans le temps pour chaque moteur. Sur Grow et Unlimited, cela montre aussi comment vous vous comparez à des concurrents nommés sur les mêmes questions.

**Trafic de référencement IA** (Grow et Unlimited) : un pixel léger et respectueux de la vie privée détecte quand une visite sur la boutique en ligne provient réellement de l'un de ces moteurs IA (via le référent, uniquement après que le visiteur a donné son consentement analytique via la bannière de cookies de votre boutique) et indique combien de visites de ce type vous avez eues au cours des 7 derniers jours — la seconde moitié de la boucle que le seul suivi de visibilité ne peut pas montrer : pas seulement « sommes-nous mentionnés », mais « cette mention envoie-t-elle quelqu'un ».

## 8. Assistance

Un assistant de chat IA est intégré à l'application (icône en bas à droite) pour répondre aux questions sur le GEO, vos résultats d'audit ou le fonctionnement d'une fonctionnalité spécifique. S'il ne peut pas vous aider, vous pouvez demander à parler à une personne et la conversation est transmise directement à IFG eCommerce.

## 9. Paramètres

C'est ici que vous gérez les réponses de l'assistant de configuration (politiques, données de l'entreprise, langue de l'interface — changez instantanément entre 30 langues, sans délai de rechargement), que vous vérifiez à nouveau l'activation du bloc de thème, et que vous consultez les scopes Shopify de votre compte.

## 10. Tarifs

**Tarifs** présente les offres Free, Grow et Unlimited côte à côte, en facturation mensuelle ou annuelle (l'offre annuelle représente environ 2 mois gratuits sur les deux offres payantes). Vous pouvez monter en gamme, rétrograder ou revenir à l'offre Free à tout moment, directement depuis l'application — aucun e-mail nécessaire. Consultez la [FAQ](faq.html) pour les limites exactes de chaque offre.

C'est le cycle complet. La plupart des marchands relancent un audit après l'ajout de nouveaux produits, vérifient le simulateur de crawler chaque fois qu'ils mettent à jour une description, et jettent un œil à la Readiness Matrix du tableau de bord chaque semaine.

[← Retour au Centre d'aide](index.html)
