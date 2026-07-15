---
title: IFG GEO Optimizer
description: Documentation, FAQ et pages légales pour l'application Shopify IFG GEO Optimizer.
lang: fr
---

# Questions fréquentes

<div class="lang-switcher">
{% include lang-switcher.html current="fr" slug="faq" %}
</div>

**Quelle est la différence entre le GEO et le SEO ?**
Le SEO traditionnel optimise pour les moteurs de recherche qui classent et listent des liens. Le GEO (Generative Engine Optimization) optimise pour les systèmes d'IA qui lisent votre contenu et génèrent directement une réponse ou une recommandation — ChatGPT, Perplexity, Gemini, Claude et Google AI Overviews. Les deux se recoupent, mais le GEO s'intéresse à des éléments que les outils SEO classiques ne vérifient pas : votre page produit dispose-t-elle de données structurées complètes, un crawler IA peut-il réellement lire votre contenu sans exécuter de JavaScript, et votre texte est-il rédigé de façon à être facile à citer.

**L'application accède-t-elle aux données de mes clients ?**
Aucune donnée personnelle de client. Les permissions Shopify de l'application sont `read_products`, `write_products`, `read_themes` et `write_pixels` — pour lire et améliorer votre catalogue, vérifier que le bloc de thème est actif, et activer un pixel anonyme de trafic de la boutique en ligne (voir ci-dessous). Elle ne demande jamais l'accès aux commandes ou aux fiches clients. Consultez la [Politique de confidentialité](privacy.html) pour le détail complet.

**Qu'est-ce que le pixel de trafic de référencement IA, et suit-il mes clients ?**
Sur Grow et Unlimited, un petit Web Pixel détecte quand une visite de la boutique en ligne arrive depuis un moteur IA reconnu (via le référent du navigateur) et indique le moteur, la page et un horodatage — rien qui identifie le visiteur, aucun cookie, aucune donnée de session. Il ne s'exécute que si le visiteur a déjà donné son consentement analytique via la bannière de cookies de votre boutique (Customer Privacy API de Shopify). Il alimente une tuile du tableau de bord (« Trafic de référencement IA, 7 derniers jours ») — le pendant du suivi Visibility AI, qui vous indique si vous êtes mentionné mais pas si cette mention a envoyé quelqu'un.

**Que change réellement le bouton « Corriger » de l'audit du catalogue ?**
Il écrit les données structurées schema.org manquantes dans un metafield du produit — des éléments comme les spécifications techniques dérivées de vos options de produit existantes. Il ne touche jamais au titre, à la description, aux images ou au prix de votre produit, et il n'invente jamais de donnée qu'il ne peut pas vérifier : un code-barres manquant, par exemple, reste manquant plutôt que d'être deviné.

**Les réponses des FAQ et les descriptions réécrites sont-elles inventées par l'IA, ou basées sur mon produit réel ?**
Le modèle ne voit que les données produit que vous avez déjà renseignées — titre, description, marque et spécifications techniques — et reçoit l'instruction explicite de ne rien ajouter qui ne figure pas dans ces données. Vous relisez chaque FAQ ou description réécrite avant sa publication ; rien n'est mis en ligne automatiquement.

**Que deviennent mes données si je désinstalle l'application ?**
La configuration de votre boutique, les audits enregistrés, les brouillons de FAQ et de réécriture de contenu, les questions de suivi de visibilité, et les événements de trafic de référencement IA sont supprimés automatiquement dès que Shopify nous notifie de la désinstallation. L'application ne conserve rien après votre départ.

**Puis-je annuler ou rétrograder sans contacter l'assistance ?**
Oui. Allez dans **Tarifs** dans l'application et passez à l'offre Free à tout moment — c'est effectif immédiatement, sans e-mail nécessaire.

## Limites des offres

| Fonctionnalité | Free | Grow | Unlimited |
|---|---|---|---|
| Audit du catalogue | 20 premiers produits, une seule fois, sans historique | Catalogue complet + historique | Catalogue complet + historique |
| Simulateur de crawler | 20/mois | 300/mois | 1 000/mois |
| Comparaison avec la concurrence | 10/mois | 50/mois | 150/mois |
| Génération de FAQ | Non inclus | 500/mois | 500/mois |
| Réécriture de contenu | Non inclus | 300/mois | 300/mois |
| Visibility AI (questions suivies) | Non inclus | 5 questions | 15 questions |
| Pixel de trafic de référencement IA | Non inclus | Inclus | Inclus |
| Chat d'assistance IA | 1 000 messages/mois | 1 000 messages/mois | 1 000 messages/mois |
| Langues de l'interface | Les 30 | Les 30 | Les 30 |

Tarifs mensuels : Free $0, Grow $9.99, Unlimited $19.99. La facturation annuelle sur Grow/Unlimited représente environ deux mois gratuits par rapport au paiement mensuel.

**Pourquoi l'offre Free ne couvre-t-elle que 20 produits ?**
Elle est conçue pour vous permettre de voir des résultats réels sur votre propre catalogue avant de vous engager sur une offre payante. Grow et Unlimited suppriment cette limite et conservent un historique complet des audits passés.

**Y a-t-il vraiment une limite sur la génération de FAQ, même sur Unlimited ?**
Oui — 500 générations par mois, délibérément, même sur l'offre la plus élevée. Cela permet de garder la fonctionnalité viable au tarif actuel ; si vous avez un catalogue à fort volume nécessitant davantage, contactez-nous et nous trouverons une solution.

**Pourquoi le chat d'assistance IA est-il identique sur toutes les offres ?**
C'est un choix produit, pas un oubli : l'assistance est incluse pour tout le monde, jamais un critère de différenciation payant. La limite de messages (1 000/mois) existe uniquement comme garde-fou technique contre les abus, pas comme une limite réelle — aucun usage légitime ne s'en approche.

**J'ai trouvé un bug ou quelque chose semble incorrect. À qui le signaler ?**
Écrivez à [info@ifgecommerce.com](mailto:info@ifgecommerce.com) en décrivant ce que vous avez constaté et, si possible, quel produit ou quelle page est concerné — c'est généralement suffisant pour identifier rapidement le problème. Vous pouvez aussi utiliser le chat d'assistance IA dans l'application et demander à parler à une personne.

[← Retour au Centre d'aide](index.html)
