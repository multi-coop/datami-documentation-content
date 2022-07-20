---
title: Tout finit par ressembler à Excel
tags: [ tech, R&D, ideas ]
created: 17/07/2022
author: Julien Paris
---

_"Il se dit"_ (du moins chez les développeurs) :

> — Tout finit par ressembler à Excel !

Peut-être que c'est le cas... Et peut-être y a-t-il des bonnes raisons à cela ? Peut-être est-ce la forme que le cerveau appréhende le mieux quand il s'agit de comprendre des listes : des formes géométriques élémentaires telles que des carrés, des lignes, des colonnes, des formes simples et claires en somme... Qu'y aurait-il de surprenant à cela ?

Est-ce vraiment que "tout ressemble à Excel" ? Ou bien est-ce qu'Excel ne ressemble-t-il pas juste à quelque chose simple à comprendre quand il s'agit de données ?

Bref... si on met l'esthétique et la philosophie de comptoir de côté, accordons-nous au moins sur le fait que **["_table is good, table gets things done_"](https://youtu.be/qUTtKYMk7u8?t=141)**.

### Des widgets pour la prévisualisation et l'édition de fichiers `csv`

Gitribute s'adresse à des utilisateurs les plus usuels qui soient (pas à des techniciens de la donnée). Donc nous n'avons pas cherché des innovations trop originales en termes d'UX. Nous voulions des interfaces que même Donald Trump serait en mesure de comprendre (même si ce n'est pas exactement le profil de _commoner_ que nous visons vraiment). Nous cherchons des interfaces accessibles et habituelles pour le plus grand nombre : 

- Une table.
- Une recherche textuelle.
- Quelques filtres.
- Pouvoir éditer.
- Pouvoir sauvegarder.
- Pouvoir télécharger les données.
- Pouvoir changer le type de visualisation si on se sent un peu aventureux.

...Simple
...[Basique](https://www.youtube.com/watch?v=2bjk26RwjyU&ab_channel=orelsan)

Une fois et seulement une fois que nous avons mis en place ces principes nous avons ajouté des ingrédients dans notre sauce de _design_ et fonctionnalités supplémentaires, notamment la possibilité de consolider des données simplement.

La principale fonctionnité un peu originale que nous avons imaginée en comparaison avec des outils de tableur classiques est celle du **bouton de consolidation** sur chaque ligne. Ce bouton permet de récupérer des données complémentaires par le biais d'APIs ("api-entreprises", "BAN api", ...) et de les injecter directement dans les données.

![GITRIBUTE-WIREFRAME-EDIT-CSV-02](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/schemas/Multi-gitribute-wireframe-edit-csv-02.png)

> **Note** : Plus de détails sur l'édition et la consolidation dans la partie **["Tutorials > Éditer un document"](/tutorial-edition)**.
