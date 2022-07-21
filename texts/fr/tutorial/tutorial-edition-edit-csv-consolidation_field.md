### Champ de consolidation

<div>
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate.png"
    />
</div>

Avec Gitribute vous pouvez paramétrer un champ à part appelé "champ de consolidation". Cette colonne sert à requêter des APis tierces afin de déléguer l'enrichissement des données du fichier à des services extérieurs à Gitrbute.

Chaque API peut être configurée indépendamment.

Une fois ce champ de consolidation correctement configuré pour un fichier source particulier, le widget affichera la colonne (ou `champ`) "consolidation" dans la colonne la plus à gauche de la table.

Chaque ligne du tableur possèdera à ce moment un bouton "consolidation" <span class="icon"><i class="mdi mdi-wrench"></i></span> dans la colonne consolidation.

En cliquant sur ce bouton tout utilisateur.rice pourra choisir entre une ou plusieurs APIs pour enrichir les données de cette ligne.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE-ROW"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate-row.png"
    />
</div>

<br>

Lorsque vous cliquez sur un des choix de consolidation / API tierce, une requête est envoyée à l'API externe et vous retourne des résultats qui apparaîtront automatiquement dans un tiroir en dessous de la ligne concernée.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE-ROW"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate-row-result.png"
    />
</div>

<br>

Ce tiroir contient les "anciennes" valeurs et les "nouvelles" :  les "anciennes" valeurs sont celles du fichier sur lequel vous travaillez, les "nouvelles" sont celles provenant de l'API.

Pour remplacer les "anciennes" valeurs par les "nouvelles", cochez simplement les champs que vous souhaitez puis cliquez sur "Valider les changements".

> **Note** : Plus de détails sur la configuration des propriétés de consolidation d'une table du widget `gitfile`, dans la partie **["Documentation > Widget 'gitfile'"](/docs-gitfile)**.
