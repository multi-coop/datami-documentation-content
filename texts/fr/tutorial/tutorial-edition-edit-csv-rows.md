### Opérations habituelles sur les lignes

<div>
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE-ROW"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/commented/tutorial-csv-edition-fr.png"
    />
</div>

<br>

Avec Gitribute vous pouvez faire un certain nombre d'opérations de base en mode "édition" :

- Modifier le contenu ou la valeur d'une cellule ;
- Ajouter une nouvelle ligne ;
- Supprimer une ligne ;
- Sélectionner une ligne ;
- Consolider une ligne (voir la prochaine partie).

Le type d'entrée d'une cellule dépend du type de `champ` (de colonne) et des propriétés de celle-ci.

L'interface d'édition d'une cellule varie essentiellement selon ce "type" :

- `text` :  soit de type `string`, chaîne de caractères
- `longtext` : longue `string`
- `number` : de type `integer`, nombre entier
- `float` : de type `float`, nombre décimal
- `boolean` ; de type `true` ou `false`
- `geopoint` : de type `float`, nombre décimal correspondant à une localisation géographique
- `tag` : de type `string` (mais une seule valeur possible parmi une liste de choix)
- `tags` : une liste de valeurs de type `string`, séparées automatiquement par un séparateur (`,` par défaut). Vous n'avez pas besoin d'écrire le séparateur entre les valeurs.

> **Note** : Nous gardons en tête qu'il serait intéressant d'inclure d'autres types, telle que `date` ou `coordinates`, nous en avons pris notre dans notre [feuille de route](/software) en particulier en prévision du cycle de développement du MVP.
