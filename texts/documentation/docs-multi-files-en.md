
## The widget `<multi-gitribute-multi-files>`

This widget allows to preview and edit a list of files stored on Gitlab or Github, or preview an explowiki.

---

### Screenshot

![multifiles](https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/screenshots/multifiles-preview-01.png)

---

### Structure

The widget takes several parameters, following this structure :

```html
  <multi-gitribute-multi-files 
    title='<YOUR-WIDGET-TITLE>'
    gitfiles='[ <MY-LIST-OF-FILES>, ... ]'
    options='{ <MY-OPTIONS> }'
    usertoken='MY-USER-TOKEN or GHOST-USER-TOKEN'
    locale='<YOUR-DEFAULT-LANGUAGE>'
  ></multi-gitribute-multi-files>
```

---

### Example

```html
  <!-- Example for loading and contribute several files into the widget -->
  <multi-gitribute-multi-files
    title="test multi-files observatoire"
    debug="false"
    locale="fr"
    options='{
      "display": "horizontal"
    }'
    gitfiles='[
      {
        "title": "Données de l&#39;observatoire",
        "activate": true,
        "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/data/csv/odf/ODF-Observatoire-apiviz_data-export_solidata-220425b-simplified.csv",
        "default-tab": true,
        "options": {
          "height": "500px",
          "separator": ";",
          "lockcolumns": true,
          "customfilters": {
            "activate": true, 
            "filterfields" : [ 
              "type",
              "platform_clean",
              "depcode"
            ]
          },
          "schema": {
            "file": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/data/json/odf/ODF-Observatoire-apiviz_data-schema.json"
          },
          "fields-custom-properties": {
            "file": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/data/json/odf/ODF-Observatoire-apiviz_data-fields-custom-props.json"
          },
          "cardsview": { 
            "activate": true,
            "default" : false
          },
          "cardsdetail": true,
          "cardssettings": {
            "mini": {
              "nom": { "position": "title" },
              "siren" : { "position": "resume" },
              "tags" : { "position": "tags" } 
            },
            "detail": {
              "nom": { "position": "title" },
              "orga": { "position": "resume" },
              "siren": { "position": "description" },
              "adress": { "position": "description" },
              "dep_label": { "position": "tags" },
              "tags" : { "position": "tags" }
            }
          }
        },
        "usertoken": ""
      },
      {
        "title": "Thématiques",
        "activate": true,
        "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/data/csv/odf/ODF-Observatoire-thematiques.csv",
        "options": {
          "height": "500px",
          "separator": ",",
          "lockcolumns": true,
          "customfilters": {
            "activate": true, 
            "filterfields" : [ 
              "Tags",
              "Organisations_Noms"
            ]
          },
          "schema": {
            "fields": [
              {
                "name": "Organisations copy",
                "type": "boolean"
              }
            ]
          },
          "fields-custom-properties": {
            "file": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/data/json/odf/ODF-thematiques-fields-custom-props.json"
          }
        },
        "onlypreview": true,
        "usertoken": ""
      },
      {
        "title": "Schéma des données de l&#39;observatoire",
        "activate": true,
        "default-tab": false,
        "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-Observatoire-apiviz_data-schema.json",
        "options": {
          "defaultDepth": 2,
          "allowKeyEdit": true
        },  
        "onlypreview": false,
        "usertoken": ""
      },
      {
        "title": "Présentation de l&#39;Observatoire de l&#39;Open data",
        "activate": true,
        "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/julien-foreign-keys/texts/markdown/odf/ODF-observatoire-intro.md",
        "options": ""
      }
    ]'>
  </multi-gitribute-multi-files>
```

---

### Widget's parameters

This widget can take several parameters, some of them depends on your input file's type (`csv`, `json`, `md`, ...)
