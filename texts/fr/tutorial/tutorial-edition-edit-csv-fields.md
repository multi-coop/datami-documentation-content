### Champs d'une table (colonnes)

Afin d'être un peu plus précis dans cette section nous dirons par la suite `champ` au lieu de parler de `colonne` d'une table.

Les champs sont listés horizontalement dans la première ligne de la table, et apparaissent dans l'ordre dans lequel ils sont écrits dans les données d'origine.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELDS"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-fields.png"
    />
</div>

<br>

Si cette option est activée dans les `options` du widget un champ peut être protégé en écriture, ceci afin d'empêcher toute modification du champ lui-même.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELD-LOCKED"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-field-locked.png"
    />
</div>

<br>

#### Champs d'une table, schéma & modèle de données, et propriétés d'une table

Avec Gitribute vous pouvez appliquer un [schéma de données](https://specs.frictionlessdata.io/table-schema/) ainsi que d'autres propriétés à votre fichier `csv` brut.

Vous pouvez voir ces propriétés pour chacun des champs juste en survolant celui-ci.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELD-TOOLTIP"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-field.png"
    />
</div>

<br>

Ces propriétés peuvent soit être "écrites en dur" dans le bloc `html`du widget, soit être écrites dans un fichier à part externe.

Les propriétés d'un champ contiennent des informations de type :

- Le **nom** du champ ;
- La **description** du champ ;
- Le **type** du champ : `string`, `boolean`, `number`, ... ;
- Ainsi que de nombreuses autres informations aidant à afficher correctement les valeurs contenues de ce champ ;

Ces informations constituent ce qu'on appelle un "schéma de données" ou "modèle de données".

Pour définir et écrire un schéma pour un fichier tabulaire nous nous référons au [standard `Table Schema`](https://specs.frictionlessdata.io/table-schema/), détaillé ici dans la documentation de [Frictionless data](https://specs.frictionlessdata.io).

En supplément du standad _Table Schema_ Gitribute peut utiliser des informations complémentaires pour décrire un champ et améliorer l'expérience utilisateur : ce type d'informations est ce que nous appelons les "propriétés _custom_" des données.

Si un schéma ou/et les propriétés _custom_ sont écrites dans des fichiers externes vous pouvez consulter ces fichiers en cliquant sur leur lien dans le dialogue "Informations sur le fichier source" (<span class="icon"><i class="mdi mdi-information-outline"></i></span>).

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELDS"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-schema_props.png"
    />
</div>

<br>

> **Note** : Plus de détails sur la façon d'appliquer un schéma de données et des propriétés _custom_ à un fichier tabulaire dans le widget `gitfile` de Gitribute, dans la partie **["Documentation > Widget 'gitfile'"](/docs-gitfile)**.
