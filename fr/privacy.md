---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
lang: fr
---

# Politique de confidentialité

<div class="lang-switcher">
{% include lang-switcher.html current="fr" slug="privacy" %}
</div>

**IFG GEO Optimizer** — une application Shopify pour l'optimisation pour moteurs génératifs (GEO)
Dernière mise à jour : juillet 2026

## 1. Responsable du traitement

Le responsable du traitement des données personnelles traitées via **IFG GEO Optimizer** est :

**IFG eCommerce** — basé à Rome, Italie
E-mail : [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Données que nous collectons

- **Données du compte marchand (via Shopify OAuth)** : le domaine de votre boutique, un jeton d'accès API, et l'adresse e-mail associée à votre compte Shopify.
- **Données du catalogue (lecture seule)** : titres, descriptions, marque, prix, options et spécifications techniques des produits — utilisés pour effectuer des audits, simuler le comportement des crawlers, évaluer l'extractibilité du contenu, et rédiger des FAQ ou des descriptions réécrites.
- **Configuration de la boutique** : votre offre active, les détails de politique de retour et d'expédition et les données d'entreprise que vous saisissez dans Paramètres, les audits enregistrés, les brouillons de FAQ et de réécriture de contenu, ainsi que les questions que vous choisissez de suivre pour la visibilité IA.
- **Messages du chat d'assistance** : le texte que vous échangez avec l'assistant IA intégré à l'application, y compris la transcription qui nous est transmise si vous demandez explicitement à parler à une personne.
- **Trafic anonyme de la boutique en ligne (Web Pixel, Grow/Unlimited)** : lorsqu'un visiteur arrive sur une page produit depuis un moteur IA reconnu (ChatGPT, Perplexity, Claude, Gemini, Copilot), nous enregistrons le moteur, l'URL de la page et un horodatage — uniquement si le visiteur a déjà donné son consentement analytique via la bannière de cookies de votre boutique. Aucun identifiant de visiteur, cookie ou donnée de session n'est collecté.
- **Données techniques** : horodatages des requêtes, identifiants internes d'enregistrement, et journaux système.

> L'application **ne demande ni ne reçoit jamais de données personnelles des clients finaux** — aucun nom, e-mail, adresse ou commande. Les permissions Shopify demandées sont `read_products`, `write_products` (catalogue et données structurées), `read_themes` (vérification de l'activation du bloc de thème), et `write_pixels` (activation du pixel de trafic anonyme mentionné ci-dessus).

## 3. Pourquoi nous les traitons, et sur quelle base légale

Nous traitons ces données pour fournir le service pour lequel vous avez installé l'application — au titre de l'art. 6(1)(b) du RGPD, exécution d'un contrat : analyser et améliorer la visibilité de votre catalogue sur les moteurs de recherche génératifs, y compris la rédaction de FAQ assistée par IA et la réécriture de contenu, le chat d'assistance intégré à l'application, le suivi hebdomadaire de la visibilité IA sur les questions que vous choisissez, et la mesure anonyme du trafic de référencement IA — toutes ces actions étant soit initiées par le marchand, soit, pour le pixel de trafic, conditionnées au consentement sur votre boutique en ligne.

## 4. Comment nous les collectons

Les données du compte sont collectées une seule fois, via le flux OAuth de Shopify, lors de l'installation. Les données du catalogue sont lues via l'API Admin de Shopify uniquement lorsque vous déclenchez une action depuis le tableau de bord. Le pixel de trafic s'exécute sur votre boutique en ligne et ne signale des événements qu'après consentement ; rien d'autre ne s'exécute en arrière-plan sans que vous ne le demandiez.

## 5. Avec qui nous les partageons

- **Google Firebase / Cloud Firestore** — stocke votre configuration, vos sessions et vos brouillons. Google LLC (États-Unis) participe au cadre de protection des données UE-États-Unis (EU-US Data Privacy Framework). Les données sont stockées dans la région europe-west1 (Belgique).
- **Anthropic PBC (États-Unis)** — fournit le modèle Claude utilisé pour la rédaction de FAQ, la réécriture de contenu et le chat d'assistance intégré à l'application, uniquement sur votre action explicite. Ne reçoit que les attributs de produit ou le texte de chat que vous fournissez — jamais de données clients.
- **OpenAI, Inc. (États-Unis)** et **Perplexity AI, Inc. (États-Unis)** — utilisés exclusivement pour le suivi hebdomadaire de la visibilité IA sur les questions que vous choisissez explicitement de surveiller. Ne reçoivent que le texte des questions suivies — jamais de données clients.
- **Google LLC (États-Unis)** — fournit le modèle Gemini, utilisé de la même manière qu'OpenAI/Perplexity ci-dessus pour le suivi de visibilité (un usage distinct de Firebase/Firestore, qui n'assure que le stockage).
- **Resend, Inc. (États-Unis)** — nous envoie une notification, avec le nom de la boutique et la transcription du chat d'assistance, uniquement lorsque vous demandez explicitement à parler à une personne dans le chat d'assistance.
- **Shopify Inc.** — la plateforme elle-même, et la source de l'API Admin et de l'infrastructure Web Pixel utilisées par l'application.

Nous ne vendons pas de données, et nous ne les utilisons ni à des fins marketing ni de profilage comportemental.

## 6. Durée de conservation

- **Jetons de session** : gérés par le cycle de vie des jetons hors ligne de Shopify, renouvelés automatiquement.
- **Configuration, audits, brouillons et événements de trafic** : conservés tant que l'application est installée. La désinstallation déclenche le webhook `shop/redact` de Shopify, qui supprime entièrement la configuration et les sessions de votre boutique.
- **Journaux techniques** : conservés selon la politique de rétention de journalisation standard de Google Cloud.

## 7. Vos droits

Conformément aux articles 15 à 22 du RGPD, vous pouvez demander l'accès à vos données, la rectification de données inexactes, ou leur suppression — le moyen le plus simple est de désinstaller l'application — ou vous opposer au traitement. Vous pouvez également déposer une plainte auprès de votre autorité locale de protection des données. Comme l'application ne traite jamais de données personnelles de clients finaux, les webhooks de conformité `customers/data_request` et `customers/redact` répondent en confirmant qu'il n'y a rien à exporter ou à supprimer.

## 8. Sécurité

Tout le trafic transite via HTTPS/TLS 1.2+. Les jetons d'authentification Shopify ne sont jamais exposés au navigateur. Chaque webhook est vérifié par un contrôle HMAC SHA-256 à temps constant avant d'être traité. La base de données n'est accessible que depuis le back-end, authentifiée via l'identité de service propre à la plateforme d'hébergement — il n'y a aucun identifiant statique dans le code, et l'accès direct depuis le client est refusé par les règles de sécurité propres à la base de données. Les données sont chiffrées au repos et en transit.

## 9. Modifications

Nous pouvons mettre à jour cette politique de temps à autre. Les modifications substantielles seront reflétées ici, avec la date en haut de page tenue à jour.

---

**Des questions sur vos données ?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Retour au Centre d'aide](index.html)
