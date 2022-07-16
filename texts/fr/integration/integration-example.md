## Integration example

Widgets can then be called directly into the page as custom html elements.

For instance to integrate a widget displaying a `csv` file you will have to copy-paste this block to your html :

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

> **Note** : A step-by-step integration tutorial for Wordpress is visible in the **["Tutorials > Wordpress integration"](/integration-wordpress)** section.
