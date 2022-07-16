<div>

  <hr>

  <!-- GITRIBUTE - contribute with GIT ...but without minding it-->
  <!-- An open source widget coded with 🤍  by the tech cooperative multi : https://multi.coop -->

  <!-- GITRIBUTE WIDGET'S HTML BLOCK-->
  <multi-gitribute-explowiki
    wikilist="https://wiki.resilience-territoire.ademe.fr/wiki/Sp%C3%A9cial:WfExplore?title=Sp%C3%A9cial%3AWfExplore&page=1&wf-expl-Category-Commun=on&wf-expl-Tags="
    options='{
      "height": "900px",
      "fields-custom-properties": {
        "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/ademe/ademe-communs-fields-custom-props.json"
      },
      "wikisettings": {
        "category": "commun",
        "fields": [
          "url",
          "description",
          "shortDescription",
          "Main_Picture",
          "Tags",
          "Theme",
          "location",
          "complement",
          "challenge",
          "commonscategorie",
          "url",
          "from"
        ],
        "tagfields": [
          "challenge",
          "Tags",
          "Theme"
        ]
      },
      "customsorting" : {
        "activate": true,
        "sortfields": [
          "title"
        ]
      },
      "customfilters" : {
        "activate": true,
        "filterfields": [
          "challenge",
          "Tags",
          "commonscategorie",
          "Theme"
        ]
      },
      "pagination": {
        "itemsPerPage": 9
      },
      "cardsview": { "activate": true, "default": true },
      "cardssettings": {
        "mini": {
          "title": {"position": "title"},
          "imageUrl": {"position": "image"},
          "shortDescription": {"position": "resume"},
          "Tags": {"position": "tags"},
          "Theme": {"position": "tags"},
          "commonscategorie": {"position": "tags"},
          "challenge": {"position": "tags"}
        },
        "detail": {
          "title": {"position": "title"},
          "imageUrl": {"position": "image"},
          "shortDescription": {"position": "resume"},
          "description": {"position": "description"},
          "complement": {"position": "description"},
          "from": {"position": "description"},
          "Tags": {"position": "tags"},
          "Theme": {"position": "tags"},
          "commonscategorie": {"position": "tags"},
          "challenge": {"position": "tags"},
          "url": {"position": "links"}
        }
      }
    }'
    title="gitribute for explowiki - communs :)"
    locale="fr"
  ></multi-gitribute-explowiki>

  <!-- GITRIBUTE WIDGET'S APP.JS SCRIPT -->
  <script src="https://gitribute.multi.coop/js/app.js" type="text/javascript"></script>

  <hr>

</div>
