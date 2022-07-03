---
title: Une stratégie R&D pour multi ? 
tags: [ multi, R&D ]
created: 10/01/2021
author: Julien Paris
---

En s'inspirant de la posture d' "éditeur" de logiciel, de quelle manière poser les bases d'une stratégie ou  d'une méthodologie lors de chaque nouveau projet ? Quel type de _checklist_ ou canevas d'analyse utiliser pour avoir une cohérence de projet en projet ? Comment s'assurer un peu contre le *bus factor* ? Je livre ici une vision personnelle, un début de réflexion, de ce que j'espère pouvoir développer au sein de la coopérative au fil des projets...

## Pourquoi cette réflexion ?

Dès les premiers jours où nous avons commencé à réfléchir à créer une coopérative pour un numérique d'intérêt général, une des idées qui me tenait à coeur et qui est **une des raisons centrales de mon engagement** est l'idée de réussir à **mutualiser des développements menés pour des clients différents**, tout en inventant notre modèle économique autour de ces solutions libres.

A l'inverse de beaucoup de personnes rencontrées dans ce milieu je pense qu'il est possible de faire des projets numériques en pensant très en amont à leur réusabilité, à leur degré de généricité, et enfin à leur potentiel pour aboutir à de réels produits libres et à produire de l'esprit d'équipe au sein de la coopérative. Cela demande surtout un peu de recul et d'huile de doigts (pour coder on se sert moins de ses coudes).

Mon souci premier est qu'on va se retrouver à suivre et développer plein de projets différents, dans des temporalités différentes, avec des équipes elles aussi différentes... si on part ainsi sans y réfléchir on va se retrouver avec des développements qui n'ont rien à voir les uns avec les autres, et surtout on aura rapidement rien à apprendre les uns des autres au sein de la coopérative...

---

La problématique que je cherche à poser se décompose ainsi :

- Comment rendre notre **offre de service claire et cohérente** ?
- Quelle(s) ligne(s) suivre pour garder **une cohérence dans les développements** ?
- Comment **capitaliser sur les développements** afin d'avoir des propositions de plus en plus convaincantes pour les clients, perdre moins de temps à chaque fois qu'on a un nouveau projet facturé ou à facturer, et permettre à d'autres membres de la coopérative de pouvoir contribuer et s'entraider ?

En s'inspirant de la posture d' "éditeur" de logiciel, de quelle manière poser les bases d'une stratégie/méthodo lors de chaque nouveau projet ? Quel type de *checklist* / canevas d'analyse utiliser pour avoir une cohérence de projet en projet ? Comment s'assurer un peu contre le *bus factor* ?

---

Voici posés de façon la plus synthétique possible les différentes choses qui me semblent aujourd'hui être importantes à garder en tête si on cherche à cheminer petit à petit vers une coopérative "éditrice de logiciels libres" et moins vers la prestation de services (type ESN ou SII).

## Une "ligne éditoriale" pour des briques logicielles (ou méthodo design) libres

- quel que soit l'outil/produit il doit être **divisible en modules interopérables** / utilisables avec un ou plusieurs des outils/produits qu'on a ou qu'on sera appelé à développer ;
- les **langages utilisés doivent pouvoir l'être par la majorité des devs**, pas de trucs trop exotiques pour assurer le passage de relais : python, js, docker, doc en français/anglais... ;
- **le socle admin sys** doit être mutualisé au max ;
- on inclut systématiquement une **réflexion sur l'XP / UX** ;
- **pas de dev sans designer** ;
- pas de produit sans **une équipe d'au moins 2 personnes** côté tech ;
- *No fork* / ***no forking way***, on cherche à généraliser le problème ;
- **pas de produit sans une stratégie** de communication, une stratégie commerciale autour du produit, et une stratégie de pérennisation ;
- **on se forme / on échange** sur tous les outils / micro-produits réalisés par la coopérative ;
- on investit dans **la documentation** ;


## Des "collections" de méso/micro-produits interopérables

- collection "**basics**" : gestion d'utilisateurs et de mots de passe, gestion ds groupes, proxies pour mailing, ...
- collection "**data**" : outils de backend + BDD de gestion de données génériques ou semi-spécialisées (données tabulaires, séries temporelle, ...) + gestion en frontend (datapatch, spreadsheep, baserow...)
- collection "**dataviz**" :  web components front de  dataviz se branchant à des micro-produits "data" ou "transformateurs"
- collection "**connecteurs**" :  interfaces entre des micro-produits "data" et des API / services externes
- collection "**transformateurs**" : intermédiaires entre des micro-produits data  et dataviz, calcul d'indicateurs (agrégation, …)
- collection "**vitrines**" : solutions pour la partie statique de sites et pas perdre de temps sur ça, voire CMS, pouvant accueillir des micro-produits front : basics, socials, dataviz...
- collection "**socials**" : outils de chat / de commentaires / de temps réel / ...
- collection "**sécurité**" : authentification / pseudonimisatiion...

---

## Quelques exemples de nos outils libres qui pourraient tendre vers des "produits"

Produits phares :

- [Apiviz](https://www.multi.coop/references?item=.%2Ftexts%2Freferences%2Fprojects%2Fapiviz.md)
- [Validata](https://www.multi.coop/references?item=.%2Ftexts%2Freferences%2Fprojects%2Fvalidata.md)
- [Data patch](https://www.multi.coop/references?item=.%2Ftexts%2Freferences%2Fprojects%2Fdata-patch.md)
- Vitrine
- [Odamap](https://www.multi.coop/references?item=.%2Ftexts%2Freferences%2Fprojects%2Faides-entreprises.md)
