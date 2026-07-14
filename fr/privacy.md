---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
---

# Privacy Policy

[← Retour au Centre d'aide](index.html)

<div class="lang-switcher">
  <a class="lang-item" href="../"><img src="../assets/flags/gb.svg" alt="" class="flag-icon">English</a>
  <a class="lang-item" href="../it/"><img src="../assets/flags/it.svg" alt="" class="flag-icon">Italiano</a>
  <a class="lang-item" href="../de/"><img src="../assets/flags/de.svg" alt="" class="flag-icon">Deutsch</a>
  <span class="lang-item lang-current"><img src="../assets/flags/fr.svg" alt="" class="flag-icon">Français</span>
  <a class="lang-item" href="../es/"><img src="../assets/flags/es.svg" alt="" class="flag-icon">Español</a>
</div>

**IFG GEO Optimizer** — une application Shopify pour l'optimisation pour moteurs génératifs (GEO)
Dernière mise à jour : juillet 2026

## 1. Responsable du traitement

Le responsable du traitement des données personnelles traitées via **IFG GEO Optimizer** est :

**IFG eCommerce**
Basé à Rome, Italie
E-mail : [ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)

## 2. Données que nous collectons

- **Données du compte marchand (via Shopify OAuth)** : le domaine de votre boutique, un jeton d'accès API, et l'adresse e-mail associée à votre compte Shopify.
- **Données du catalogue (lecture seule)** : titres, descriptions, marque, prix, options et spécifications techniques des produits — utilisés pour effectuer des audits, simuler le comportement des crawlers, évaluer l'extractibilité du contenu et rédiger des FAQ.
- **Configuration de la boutique** : votre offre active, les détails de politique de retour et d'expédition que vous saisissez dans Paramètres, ainsi que tout brouillon ou approbation de FAQ que vous créez.
- **Données techniques** : horodatages des requêtes, identifiants internes d'enregistrement, et journaux système.

> L'application ne demande ni ne reçoit jamais de données des clients finaux — aucun nom, e-mail, adresse ou commande. Les seules permissions Shopify demandées sont `read_products` et `write_products`.

## 3. Pourquoi nous les traitons, et sur quelle base légale

Nous traitons ces données pour fournir le service pour lequel vous avez installé l'application — au titre de l'art. 6(1)(b) du RGPD, exécution d'un contrat : analyser et améliorer la visibilité de votre catalogue sur les moteurs de recherche génératifs (ChatGPT, Perplexity, Gemini, Google AI Overviews), y compris la rédaction de FAQ lorsque vous le demandez explicitement.

## 4. Comment nous les collectons

Les données du compte sont collectées une seule fois, via le flux OAuth de Shopify, lors de l'installation de l'application. Les données du catalogue sont lues via l'API Admin de Shopify uniquement lorsque vous déclenchez une action — une analyse, une simulation, ou une génération de FAQ — depuis le tableau de bord de l'application. Rien ne s'exécute en arrière-plan sans que vous ne le demandiez.

## 5. Avec qui nous les partageons

- **Google Firebase / Cloud Firestore** — stocke la configuration de votre boutique, les sessions et les brouillons de FAQ. Google LLC (États-Unis) participe au cadre de protection des données UE-États-Unis (EU-US Data Privacy Framework). Les données sont stockées dans la région europe-west1 (Belgique).
- **Anthropic PBC (États-Unis)** — fournit le modèle de langage (Claude) utilisé pour rédiger les suggestions de FAQ, uniquement lorsque vous demandez explicitement une génération. Elle ne reçoit que les attributs de produit que vous avez déjà saisis — titre, description, marque, spécifications — jamais de données clients. Consultez la politique de confidentialité et les conditions commerciales d'Anthropic pour savoir comment ces données sont traitées.
- **Shopify Inc.** — la plateforme elle-même, et la source de l'API Admin utilisée par l'application.

Nous ne vendons pas de données, et nous ne les utilisons ni à des fins marketing ni de profilage comportemental.

## 6. Durée de conservation

- **Jetons de session** : gérés par le cycle de vie des jetons hors ligne de Shopify, renouvelés automatiquement.
- **Configuration, audits et brouillons de FAQ** : conservés tant que l'application est installée. La désinstallation déclenche le webhook `shop/redact` de Shopify, qui supprime entièrement la configuration et les sessions de votre boutique.
- **Journaux techniques** : conservés selon la politique de rétention de journalisation standard de Google Cloud.

## 7. Vos droits

Conformément aux articles 15 à 22 du RGPD, vous pouvez demander l'accès à vos données, la rectification de données inexactes, ou leur suppression — le moyen le plus simple est de désinstaller l'application — ou vous opposer au traitement. Vous pouvez également déposer une plainte auprès de votre autorité locale de protection des données. Comme l'application ne traite jamais de données de clients finaux, les webhooks de conformité `customers/data_request` et `customers/redact` répondent en confirmant qu'il n'y a rien à exporter ou à supprimer.

## 8. Sécurité

Tout le trafic transite via HTTPS/TLS 1.2+. Les jetons d'authentification Shopify ne sont jamais exposés au navigateur. Chaque webhook est vérifié par un contrôle HMAC SHA-256 à temps constant avant d'être traité. La base de données n'est accessible que depuis le back-end, authentifiée via l'identité de service propre à la plateforme d'hébergement — il n'y a aucun identifiant statique dans le code, et l'accès direct depuis le client est refusé par les règles de sécurité propres à la base de données. Les données sont chiffrées au repos et en transit.

## 9. Modifications

Nous pouvons mettre à jour cette politique de temps à autre. Les modifications substantielles seront reflétées ici, avec la date en haut de page tenue à jour.

---

**Des questions sur vos données ?**
[ifgecommerce@gmail.com](mailto:ifgecommerce@gmail.com)
