## Éditer un fichier JSON

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-JSON"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edition-edit-json.png"
    />
</div>

<br> 

Le widget `gitfile` de Gitribute permet également d'éditer un fichier de type `json` (et donc évidemment un fichier `geojson`).

Vous disposerez d'exactement les mêmes "vues-édition" lors de l'édition d'un `json`que pour les fichiers : vues `prévisualisation` / `édition` / `diff`.

Un objet `json` est constitué de `noeuds`que vous pouvez replier ou déplier.

Un `json` possède un niveau "racine" ("root"). Au niveau de la raciine vous pouvez trouver soit un `noeud` soit une `liste` de `noeuds`.

Un `noeud` peut contenir différents types d'objets :

- Un autre `noeud` ;
- Un `objet` standard : `string`, `number`, `object`, `boolean` ;
- Une `liste` (`array`) d'objets ou de `noeuds`. Si un `noeud` fait partie d'une liste son index dans la `liste` fait office de nom.

Le type du `noeud` est symbolisé par une petite icône rouge après le nom du `noeud`:

- `{}` : `object` (`objet`)
- `[]` : `array` (`liste`)
- `abc` : `string` (chaîne de caractères)
- `123` : `number` (nombre) or `float` (nombre décimal)
- `☑️` : `boolean` (bouléen, `true` ou `false`)

En mode édition d'un fichier `json` vous pouvez :

- Ajouter un nouveau `noeud`, en cliquant sur l'icône `+`.
- Supprimer un `noeud`, en cliquant sur l'icône `trash`.
- Modifier un `noeud` :
  - Changer la clé d'un `noeud` si le `noeud` n'est pas un élément d'une `liste`, en cliquant sur l'icône `pen` <span class="icon"><i class="mdi mdi-pencil"></i></span>.
  - Changer la valeur d'un `noeud`

Le tout de manière récursive...

> **Note** : Les fichiers `json` sont très utiles pour décrire des données non tabulaires ("non structurées"), mais il est également possible de valider des fichiers `json` étant donné un schéma de référence. 
>
> Dans la coopérative [multi](https://multi.coop) nous travaillons d'ailleurs sur un [validateur json](https://git.opendatafrance.net/outillages/json-validator) qui vous intéressera certainement si vous arrivé.e jusqu'ici dans la documentation.
>
> Petit tuyau de _nerd_ à _nerd_...
