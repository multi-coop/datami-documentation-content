<div>

  <hr>

  <!-- GITRIBUTE - contribute with GIT ...but without minding it-->
  <!-- An open source widget coded with 🤍  by the tech cooperative multi : https://multi.coop -->

  <!-- GITRIBUTE WIDGET'S HTML BLOCK-->
  <multi-gitribute-file
    title="ODF - Ressources (export airtable)"
    gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-liste des ressources.csv"
    options='{
      "height": "500px",
      "separator": ",",
      "lockcolumns": true,
      "tagseparator": ",",
      "customfilters": {
        "activate": true,
        "filterfields": [
          "Type",
          "Enjeux politiques",
          "Enjeux Opérationnels",
          "Phase"
        ],
        "tagsSeparator": ","
      },
      "schema": {
        "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-ressources-schema.json"
      },
      "fields-custom-properties": {
        "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-ressources-fields-custom-props.json"
      },
      "customsorting": {
        "activate": true,
        "sortfields": [
          "Objet",
          "Nom de la ressource"
        ]
      },
      "pagination": {
        "itemsPerPage": 20
      },
      "cardsview": {
        "activate": true,
        "default": false
      },
      "cardsdetail": true,
      "cardssettings": {
        "mini": {
          "Nom de la ressource": {
            "position": "title"
          },
          "Objet": {
            "position": "resume"
          },
          "Enjeux politiques": {
            "position": "tags"
          },
          "Phases": {
            "position": "tags"
          }
        },
        "detail": {
          "Nom de la ressource": {
            "position": "title"
          },
          "Objet": {
            "position": "resume"
          },
          "Enjeux politiques": {
            "position": "tags"
          },
          "Phases": {
            "position": "tags"
          },
          "Lien vers la ressources": {
            "position": "links"
          }
        }
      }
    }'
    onlypreview="false"
    locale="fr"
  ></multi-gitribute-file>

  <!-- GITRIBUTE WIDGET'S APP.JS SCRIPT -->
  <script src="https://gitribute.multi.coop/js/app.js" type="text/javascript" defer></script>

  <hr>

</div>
