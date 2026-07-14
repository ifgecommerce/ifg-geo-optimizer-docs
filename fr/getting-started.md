---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
---

# Prise en main

[← Retour au Centre d'aide](index.html)

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <span class="lang-item lang-current"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</span>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

Ce guide couvre tout, de l'installation de l'application à la publication de votre première FAQ optimisée pour l'IA.

## 1. Installer et ouvrir le tableau de bord

Une fois installée, IFG GEO Optimizer s'ouvre directement dans votre back-office Shopify. Le tableau de bord est votre point de départ — il se remplit avec le score GEO de votre boutique et votre activité récente au fur et à mesure que vous utilisez l'application.

## 2. Renseigner vos politiques

Allez dans **Paramètres** et saisissez les détails de votre politique de retour et d'expédition (délai de retour, qui paie les frais de retour, délais de traitement et de transit, pays de destination). Ces informations alimentent directement les données structurées que l'application publie pour chaque produit — les pages produit de Shopify n'exposent pas ces informations aux moteurs de recherche autrement, donc cette seule étape améliore de manière mesurable votre score d'audit.

## 3. Lancer votre premier audit de catalogue

Ouvrez **Audit du catalogue** et cliquez sur **Réanalyser le catalogue**. L'application lit votre catalogue de produits via l'API Admin de Shopify et vérifie chaque produit sur neuf champs de données structurées recherchés par les moteurs de recherche : image, description, marque, référence (SKU), GTIN, prix, spécifications techniques, politique de retour et politique d'expédition.

Les produits en dessous de 80/100 montrent exactement ce qui manque. Lorsque l'application peut le corriger automatiquement — généralement en dérivant les spécifications techniques de vos options de produit existantes — vous verrez un bouton **Corriger**. Un seul clic écrit les données schema.org manquantes directement sur le produit ; rien n'est deviné ou inventé pour les champs que l'application ne peut pas dériver de manière fiable (un code-barres, par exemple, n'est jamais généré automatiquement).

Sur l'offre Gratuite, les audits couvrent vos 20 premiers produits et ne conservent pas d'historique. Les offres Grow et Unlimited couvrent tout votre catalogue et enregistrent chaque analyse.

## 4. Activer le bloc de thème

Les données structurées corrigées par votre audit n'apparaissent pas sur votre boutique en ligne tant que vous ne les avez pas activées. Dans l'éditeur de thème, allez dans **Extensions d'application** et activez **GEO Schema**. C'est une activation unique — ensuite, chaque page produit inclut automatiquement le JSON-LD généré par votre audit.

## 5. Vérifier ce qu'un bot voit réellement

Ouvrez **Crawler IA** et choisissez un produit. L'application récupère la page exactement comme le ferait un crawler IA — sans exécution JavaScript, comme GPTBot, ClaudeBot ou PerplexityBot — pour que vous puissiez voir précisément ce qui est visible pour ces moteurs, y compris si votre fichier robots.txt les bloque et si vos données structurées sont complètes dans le HTML brut.

## 6. Générer des FAQ

Sur les offres Grow ou Unlimited, ouvrez **FAQ produit**, choisissez un produit, puis cliquez sur **Générer 3 FAQ**. L'application rédige trois paires question-réponse à partir du titre, de la description et des spécifications réels de votre produit — jamais de détails inventés. Relisez chaque brouillon, puis **Approuver et publier** ceux que vous souhaitez mettre en ligne ; les FAQ approuvées apparaissent sur votre page produit et sont balisées en données structurées FAQPage pour les moteurs de recherche. Rien n'est publié sans votre relecture.

## 7. Choisir une offre

**Tarifs** présente les offres Gratuite, Grow et Unlimited côte à côte, avec facturation mensuelle et annuelle. Vous pouvez changer d'offre ou revenir à l'offre Gratuite à tout moment, directement depuis l'application — pas besoin de contacter l'assistance pour rétrograder.

C'est le cycle complet. La plupart des marchands relancent un audit après l'ajout de nouveaux produits, et vérifient le simulateur de crawler chaque fois qu'ils mettent à jour une description de produit.
