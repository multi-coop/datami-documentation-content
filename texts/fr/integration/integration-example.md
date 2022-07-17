## Exemple d'intégration

Les widgets peuvent être insérés et personnalisés dans une page web.

L'exemple suivant vous montre le code ˋhtmlˋ d'un widget affichant un fichier ˋcsvˋ. Vous pouvez copier-coller ce bloc dans une page html de votre choix : 

```html
<!-- GITRIBUTE - contribute with GIT ...but without minding it-->
<!-- An open source widget coded with 🤍  by the tech cooperative multi : https://multi.coop -->

<!-- GITRIBUTE WIDGET -->
<multi-gitribute-file
  title="gitribute for gitlab file - csv (comma separator)" 
  gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/test-table-comma.csv" 
  options='{
    "separator": ","
    "pagination": {
      "itemsPerPage": 5
    },
    "cardsview": {
      "activate": true,
      "default": true
    },
    "cardsdetail": true,
    "cardssettings": {
      "mini": {
        "name": {"position": "title"},
        "surname": {"position": "title"},
        "profession": {"position": "resume"}
      },
      "detail": {
        "name": {"position": "title"},
        "surname": {"position": "title"},
        "profession": {"position": "desription"}
      }
    }
  }' 
  usertoken="MY-USER-TOKEN or GHOST-USER-TOKEN"
  locale="en"
  debug="false"
></multi-gitribute-file>

<!-- GITRIBUTE WIDGET'S APP.JS SCRIPT -->
<script src="https://gitribute.multi.coop/js/app.js" type="text/javascript" defer></script>
```

> **Note** : Un tutoriel étape par étape pour intégrer un widget dans Wordpress est acessible dans la partie **["Tutoriels > Intégration Wordpress"](/integration-wordpress)**.
