---
title: Architecture & sketches
tags: [ tech, R&D ]
created: 17/07/2022
author: Julien Paris
---

Comment s'opère la transition entre :

> — _Hé, on devrait pas utiliser Git dans des projets frontend ?_

 et :

> — _[Monsieur, auriez-vous une minute pour parler de Gitribute ?](https://www.youtube.com/watch?v=sghOYbR_fXA&ab_channel=TikTokTaciousShorts)_

Cette partie se focialise sur les travaux préparatoire et le _brainstorming_ qui ont permis de passer d'une bonne idée encore floue au projet Gitribute tel qu'il est aujourd'hui : [un plan, une feuille de route, une architecture "agile"](https://www.linkedin.com/pulse/agile-approach-methodology-carlo-occhiena/).

"_There's no wizard jizz in [making stuff](https://www.youtube.com/watch?v=N4IfPtl3W_M&ab_channel=exurb1a), [only a lot of engineering](https://www.youtube.com/watch?v=qE0UimODxNg&ab_channel=exurb1a)_"

C'est parti pour un petit trip...

## Sketches & wireframes

Gitribute posséde quelques fonctions et composants principaux (_core_), réutilisables par d'autres composants.

Les fonctions _core_ sont stockées dans le répertoire `utils` : requêtes des APIs, conversion d'un csv brut à un objet javascript, etc...

Les données du _front_ sont stockées dans un _vuex store_ : langue, infos utilisateurs, branche de travail, metadonnées des fichiers, etc... sont stockées à cet endroit.

Enfin certains _composants complexes peuvent être réutilisés_ par d'autres, tels que les composants `EditCell` ou `GitributeTable`, qui sont réutilisés autant par les composants de haut niveau `explowiki` que `gitfile` dans leur partie table.

Nous sommes fiers (et un peu gênés aussi) d'affirmer notre `#passionSchema`...

![SCHEMA-GITRIBUTE-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-schema-02.png)

> **Note** : Plus de détails sur les widgets dans la partie **["Documentation > Panorama"](/docs-widgets-overview)**.

## Components wireframes

🚧  &nbsp; `Translation in progress...`

Gitribute started with an idea, while sitting at a cafe near Paris, outside, with a bright sun on a sunny sunday. No laptop around.

We started designing Gitribute a bit in an "old-fashion" way : with a pen and a paper. No fancy tools like Figma at this precise moment at the cafe.

Keeping on with this approach the "wireframes" you will se below are more ideas or sketches than real design canvases. But drawing can still be relevant and more straight-to-the-point, even in the digital world.

After all, how did they build those pyramids, any building, any painting, anything needing a bit of planning... before the computers ?

### Widget for `md` preview and edition

🚧  &nbsp; `Translation in progress...`

We were inspired a lot by [HedgeDoc](https://hedgedoc.org/) and [Hackmd](https://hackmd.io) interfaces.

**The only thing we added was `diff` view**, as an intermediary between preview and edition.

![GITRIBUTE-WIREFRAME-EDIT-MD-01](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-wireframe-edit-md-01.png)

> **Note** : More about editing and diff view in the **["Tutoriels > Éditer un document"](/tutorial-edition)** section

## Dialog before saving changes (send a contribution)

🚧  &nbsp; `Translation in progress...`

To "save" one's changes over a data, we use Git for version control.

More precisely we rely on Git service providers like Github or Gitlab. 

The [Git syntax](https://en.wikipedia.org/wiki/Git) could seem a bit tricky at first sight.

"Merge requests", "branches" and this kind of weirds notions are not terms your grandma' or grandpa' are _really_ interested in.

_( If they seem to, call a doctor.)_

At the contrary _"saving"_, a document became something quite usual for most humans in the XXIth century.

**"Contributing" lays halfway between the tech world and common cultural habits.**

The challenge was to find an "user path" - and a design - to express this intention **simply** and **honestly** :

- "Simply" by avoiding any dispensable information, straight to the point ;
- "Honestly" by letting the user learn step by step what those weird terms (tooltips), keeping technical information in the background (in another tab, but accessible), etc...

![GITRIBUTE-WIREFRAME-DIALOG_SAVE-01](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-wireframe-commit_dialog-01.png)

That said it is not completly useless to have a basic understanding of Git, and [many](https://www.atlassian.com/git) [websites](https://learngitbranching.js.org/?locale=fr_FR), [videos](https://www.youtube.com/watch?v=2ReR1YJrNOM&ab_channel=ProgrammingwithMosh), or sometimes people are available to learn the basics.

> **Note** : More about contributing in the **["Tutorials > Contribute to a document"](/tutorial-contribution)** section
