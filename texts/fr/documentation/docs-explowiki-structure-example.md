### Exemple

```html
  <!-- Example for loading and contribute to a distant mediawiki ressource -->
  <multi-gitribute-explowiki
      wikilist="https://wiki.lafabriquedesmobilites.fr/wiki/Sp%C3%A9cial:WfExplore?title=Sp%C3%A9cial%3AWfExplore&page=1&wf-expl-Category-Projet=on&wf-expl-Page_creator-fulltext=&wf-expl-Tags="
      wikipages='[
        "https://wiki.lafabriquedesmobilites.fr/wiki/Accra_Mobile",
        "https://wiki.lafabriquedesmobilites.fr/wiki/Agremob_Self_Data_Territorial_La_Rochelle",
        "https://wiki.lafabriquedesmobilites.fr/wiki/Autonomous_Kart_for_Student"
      ]'
      options='{
        "wikisettings": {
          "category": "projet",
          "fields": [
            "url",
            "description",
            "shortDescription",
            "Main_Picture",
            "Coordonnées géo",
            "needs",
            "referent",
            "communauté d&#39;intérêt",
            "Titre",
            "Tags",
            "etape",
            "Theme",
            "location",
            "from",
            "challenge"
          ],
          "tagfields": [
            "Tags",
            "Theme",
            "location",
            "from",
            "challenge"
          ]
        },
        "pagination": {
          "itemsPerPage":12
        },
        "cardsview": {
          "activate": true,
          "default": true
        },
        "cardssettings": {
          "mini": {
            "title": {"position": "title"},
            "imageUrl": {"position": "image"},
            "shortDescription": {"position": "resume"}
          },
          "detail": {
            "title": {"position": "title"},
            "imageUrl": {"position": "image"},
            "shortDescription": {"position": "resume"},
            "description": {"position": "description"}
          }
        }
    }'
    title="gitribute for gitlab file - csv (comma separator)" 
    usertoken="MY-USER-TOKEN or GHOST-USER-TOKEN"
    locale="en"
    debug="false"
  ></multi-gitribute-explowiki>
```
