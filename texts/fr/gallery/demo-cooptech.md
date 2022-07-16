<div>

  <hr>

  <!-- GITRIBUTE - contribute with GIT ...but without minding it-->
  <!-- An open source widget coded with 🤍  by the tech cooperative multi : https://multi.coop -->

  <!-- GITRIBUTE WIDGET'S HTML BLOCK-->
  <multi-gitribute-file
    title="Liste des coopératives de la tech en France - csv ( semicolon separator)"
    gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/cooptech/Annuaire-SCOP-SCIC-tech-France.csv"
    options='{
      "height": "500px",
      "separator": ",",
      "lockcolumns": true,
      "tagseparator": ",",
      "customfilters": {
        "activate": true,
        "filterfields": [
          "type",
          "Statut juridique"
        ],
        "tagsSeparator": ","
      },
      "schema": {
        "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-schema.json"
      },
      "fields-custom-properties": {
        "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-fields-custom-props.json"
      },
      "customsorting": {
        "activate": true,
        "sortfields": [
          {
            "name": "Nom"
          }
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
          "Nom": {
            "position": "title"
          },
          "Présentation": {
            "position": "description"
          },
          "Site internet": {
            "position": "description"
          },
          "Statut juridique": {
            "position": "tags"
          },
          "Domaine(s)": {
            "position": "tags"
          }
        },
        "detail": {
          "Nom": {
            "position": "title"
          },
          "Site internet": {
            "position": "description"
          },
          "Présentation": {
            "position": "description"
          },
          "Numéro SIREN": {
            "position": "description"
          },
          "Adresse": {
            "position": "description"
          },
          "Statut juridique": {
            "position": "tags"
          },
          "Domaine(s)": {
            "position": "tags"
          },
          "Fiche URSCOP": {
            "position": "links"
          }
        }
      }
    }'
    onlypreview="false"
    locale="fr"
  ></multi-gitribute-file>

  <!-- GITRIBUTE WIDGET'S APP.JS SCRIPT -->
  <script src="https://gitribute.multi.coop/js/app.js" type="text/javascript"></script>

  <hr>

</div>
