---
title: Comment ça marche Datami ?
tags: [ tech, R&D ]
created: 17/07/2022
author: Julien Paris
---

C'est parti pour un petit coup d'oeil sous le capot.

## Datami est une collection de widgets

Datami est une application web fournissant une série de "[widgets](https://en.wikipedia.org/wiki/Web_widget)". Cela signifie que **vous pouvez intégrer Datami dans n'importe quel site web**, et que vous n'avez pas besoin de votre propre serveur pour utiliser un widget de Datami.

Le terme "widget" est équivalent à celui de "composant web", c'est une façon d'afficher au sein d'un site un composant indépendant fourni par un serveur tiers. L'approche "widget" est similaire à celle de la bonne vieille _iframe_, à ceci près que les widgets sont plus flexibles et plus adaptés au web d'aujourd'hui que les _iframes_.

## Datami s'appuie sur des "services Git"

La différence fondamentale de Datami avec des solutions propriétaires (type GoogleSheet ou Airtable) et leurs équivalents libres (comme [nocoDB](https://www.nocodb.com/) ou [Baserow](https://baserow.io/)) est que la donnée que vous éditez avec Datami n'est pas stockée sur _nos_ serveurs.

Vos données est stockée là où vous le souhaitez, par exemple sur votre propre instance Gitlab ou dans votre propre compte / organisation Github.

**Datami n'a pas de serveur, pas de _backend_**, mais s'adosse à des services largement populaires comme [Gitlab](https://gitlab.com/), [Github](https://github.com/), ou [Mediawiki](https://www.mediawiki.org/wiki/MediaWiki) pour l'hébergement de vos données. Les APIs de ces "services Git" permettent de les visualiser et d'opérer des modifications dessus à distance.

Cela signifie que si vous avez déjà un compte sur Gitlab (ou encore mieux que vous avez votre propre instance Gitlab) vous n'avez pas à louer un serveur supplémentaire pour héberger vos données. Vous pouvez laisser vos données là où elles se trouvent (Gitlab / Github / Mediawiki), et c'est très bien ainsi car ces services Git peuvent déjà faire énormément de choses utiles : garder un historique des versions, l'authentification, la gestion des droits, gérer les `pull requests`...

De cette façon les données restent hébergées et protégées, et vous pouvez gérer les propositions de contributions entrantes comme vous géreriez n'importe quelle `pull request` : en vérifiant la qualité de la proposition, en l'acceptant ou la refusant, et c'est tout.

> **Note** : Plus de détails sur notre _benchmark_ de solutions d'édition de données "no-code" dans la partie **["Pourquoi Datami ? > Benchmark"](/benchmark)**.

## Contribuer anonymement (pour les timides)

Datami utilise le système de [jetons personnels (ou _tokens_)](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) fourni par Github et Gitlab pour faire des sauvegardes (ou "commit") et contribuer à des données hébergées sur leurs services.

Pour éviter d'avoir à demander à votre papi ou votre mamie de se créer un compte sur ces outils (ou pire d'avoir à leur demander de se créer un _token_), **Datami utilise par défaut un _token_ "fantôme"**.

Si vous voulez permettre à des utilisateurs de faire des contributions anonymement sur vos données il est nécessaire de configurer avec attention votre _repository_ Github ou Gitlab pour qu'il accepte des actions (PUT, POST, GET) venant de cet utilisateur "fantôme".

> **Note** : Par exemple vous ne souhaitez certainement pas que cet utilisateur "fantôme" puisse faire des "pushes" directement sur votre branche `main`...

Pour résumer, lorsque vous configurez votre widget Datami en partant de zéro vous devez :

- 1/ Créer un utilisateur "fantôme" et son _token_ ;
- 2/ Configurer votre _repo_ cible sur votre service Git pour que votre _repo_ accepte les contributions de l'utilisateur "fantôme" : celui-ci doit pouvoir y créer de nouvelles branches et y faire des _commits_, sauf pour la branche `main`) ;
- 3/ Indiquer ce jeton "fantôme" dans le widget Datami (soit dans le fichier `.env`, soit dans le `html` du widget)

De cette manière **un utilisateur peut alors faire des _commits_ anonymement, sans avoir à se créer un compte sur Github ou Gitlab**. Cet utilisateur anonyme peut toutefois choisir de laisser un petit message au propriétaire des données et/ou indiquer son mail.

Les utilisateurs plus familiers de Git peuvent aussi utiliser leur propre _token_.

Vos données sur la branche principale (en général `main` ou `master`) restent ainsi protégées, et vous - le.la propriétaire des données source - gardez le contrôle complet sur qui peut écrire et sur quelle branche.

C'est un petit _hack_, mais le "truc" de l'utilisateur fantôme n'est au final pas aussi compliqué que cela : c'est un peu comme laiser une connaissance utiliser votre compte Netflix.
