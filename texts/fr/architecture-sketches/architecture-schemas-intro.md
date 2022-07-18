# Architecture & dessins

Comment s'opère la transition entre :

> — _Hé, on devrait pas utiliser Git dans des projets frontend ?_
 
 et :
 
> — _[Monsieur, auriez-vous une minute pour parler de Gitribute ?](https://www.youtube.com/watch?v=sghOYbR_fXA&ab_channel=TikTokTaciousShorts)_

Cette partie se focialise sur les travaux préparatoire et le _brainstorming_ qui ont permis de passer d'une bonne idée encore floue au projet Gitribute tel qu'il est aujourd'hui : [un plan, une feuille de route, une architecture "agile"](https://www.linkedin.com/pulse/agile-approach-methodology-carlo-occhiena/).

_There's no wizard jizz in [making stuff](https://www.youtube.com/watch?v=N4IfPtl3W_M&ab_channel=exurb1a), [only a lot of engineering](https://www.youtube.com/watch?v=qE0UimODxNg&ab_channel=exurb1a)_

C'est parti pour un petit trip...

## Sketches & wireframes

Gitribute posséde quelques fonctions et composants principaux (_core_), réutilisables par d'autres composants.

Les fonctions _core_ sont stockées dans le répertoire `utils` : requêtes des APIs, conversion d'un csv brut à un objet javascript, etc...

Les données du _front_ sont stockées dans un _vuex store_ : langue, infos utilisateurs, branche de travail, metadonnées des fichiers, etc... sont stockées à cet endroit.

Enfin certains _composants complexes peuvent être réutilisés_ par d'autres, tels que les composants `EditCell` ou `GitributeTable`, qui sont réutilisés autant par les composants de haut niveau `explowiki` que `gitfile` dans leur partie table.

Nous sommes fiers (et un peu gênés aussi) d'affirmer notre `#passionSchema`...

![SCHEMA-GITRIBUTE-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-schema-02.png)

> **Note** : Plus de détails sur les widgets dans la partie **["Documentation > Panorama"](/docs-widgets-overview)**.
