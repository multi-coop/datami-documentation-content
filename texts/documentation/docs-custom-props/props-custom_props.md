## Custom properties file

🚧  &nbsp; `Redaction in progress...`

### Structure

```json
{
  "fields": [],
  "consolidation": [],
  "validation": []
}
```

### Custom fields properties

🚧  &nbsp; `Redaction in progress...`

#### Example

```json
{
    "fields": [
    {
      "name": "id_odf",
      "locked": true
    },
    {
      "name": "nom",
      "sticky": true
    },
    {
      "name": "siren"
    },
    {
      "name": "adress",
      "subtype": "longtext",
      "maxLength": 15
    },
    {
      "name": "id_datagouv",
      "hide": true
    },
    {
      "name": "type",
      "subtype": "tag",
      "definitions": [
        {
          "value": "AGCT",
          "label": "Autre Groupement de Collectivités Territoriales",
          "description": "SMI, GIP, ..."
        },
        {
          "value": "CA",
          "label": "Communauté d'Agglomération"
        },
        {
          "value": "CC",
          "label": "Communauté de Communes"
        },
        {
          "value": "COM",
          "label": "Commune"
        },
        {
          "value": "CU",
          "label": "Communauté Urbaine"
        },
        {
          "value": "DEP",
          "label": "Département"
        },
        {
          "value": "DSPT",
          "label": "Délagataire de Services Publics Territoriaux",
          "description": "opérateurs privés, Soc. d'Economie Mixte,..."
        },
        {
          "value": "EPT",
          "label": "Etablissement Public Territorial",
          "description": "rattaché à la Métropole du Grand Paris"
        },
        {
          "value": "MET",
          "label": "Métropole"
        },
        {
          "value": "OACT",
          "label": "Organisme Associé de Collectivité Territoriale",
          "description": "Office de Tourisme, Régie de transport, ..."
        },
        {
          "value": "REG",
          "label": "Région"
        },
        {
          "value": "SDE",
          "label": "..."
        }
      ]
    },
    {
      "name": "thématiques",
      "subtype": "tags",
      "tagSeparator": "-",
      "bgColor" : "#BED3C3",
      "foreignKey": {
        "activate": true,
        "ressource": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-Observatoire-thematiques.csv",
        "fields": "Thématique",
        "returnFields" : [
          "Tags"
        ]
      }
    },
    {
      "name": "merge",
      "subtype": "tags",
      "tagSeparator": "+",
      "definitions": [
        {
          "value": "ptf",
          "label": "Publication sur un portail local"
        },
        {
          "value": "datagouv",
          "label": "Publication sur le portail data.gouv"
        }
      ]
    },
    {
      "name": "orga",
      "subtype": "tag",
      "allowNew": true,
      "bgColor" : "#F0BE86"
    },
    {
      "name": "platform_clean",
      "subtype": "tag"
    },
    {
      "name": "depcode",
      "subtype": "tag",
      "foreignKey": {
        "activate": true,
        "ressource": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-Observatoire-departements-regions.csv",
        "ressourceOptions": {
          "separator": ","
        },
        "fields": "depcode",
        "returnFields" : [
          "Département",
          "région"
        ]
      }
    },
    {
      "name": "reg_code_geo",
      "subtype": "tag"
    },
    {
      "name": "reg_code_short",
      "subtype": "tag"
    },
    {
      "name": "tranche_ptf",
      "subtype": "tag"
    },
    {
      "name": "tranche_pop",
      "subtype": "tag"
    },
    {
      "name": "url_ptf",
      "subtype": "link"
    },
    {
      "name": "url_datagouv",
      "subtype": "link"
    }
  ]
}
```

### Consolidation properties

🚧  &nbsp; `Redaction in progress...`

#### Example

```json
{
  "consolidation": [,
    {
      "api_name": "adresse.gouv.fr",
      "source_fields": [
        { "name": "adress" }
      ],
      "activate": true,
      "api": "https://api-adresse.data.gouv.fr/search/?q={{adress}}",
      "results_fields": [
        { 
          "resp_field" : "features.0.geometry.coordinates.1",
          "map_to_field": "lat"
        },
        { 
          "resp_field" : "features.0.geometry.coordinates.0",
          "map_to_field": "lon"
        }
      ]
    }
  ]
}
```

### Validation

🚧  &nbsp; `Redaction in progress...`
