
## How to integrate your customized Gitribute widgets

### Dependencies

Gitribute's widgets need three files in order to work correctly :

- `app.js` : the Gitribute application itself
- `app.css` : Gitribute's styles
- `materialdesignicons-webfont.woff2`: : Gitribute's icons

### Imports

Add those files to your html head, like this if the widget code is deployed on `https://gitribute.multi.coop`:

```html
<!-- IMPORT THE WIDGETS APP FILE -->
<script src="https://gitribute.multi.coop/js/app.js" type="text/javascript"></script>

<!-- IMPORT THE WIDGETS CSS FILES -->
<link type="text/css" href="https://gitribute.multi.coop/js/app.css" rel="stylesheet">
<link type="text/css" href="https://gitribute.multi.coop/fonts/materialdesignicons-webfont.woff2" rel="stylesheet">

```

### Integration examples

Widgets can then be called directly into the page as custom html elements.

For instance to integrate a widget displaying a `csv` file you will have to copy-paste this block to your html :


```html
<!-- IMPORT THE WIDGETS APP FILE -->
<script src="https://gitribute.multi.coop/js/app.js" type="text/javascript"></script>

<!-- IMPORT THE WIDGETS CSS FILES -->
<link type="text/css" href="https://gitribute.multi.coop/js/app.css" rel="stylesheet">
<link type="text/css" href="https://gitribute.multi.coop/fonts/materialdesignicons-webfont.woff2" rel="stylesheet">

<!-- GITRIBUTE WIDGET -->
<multi-gitribute-file
  title="gitribute for gitlab file - csv (comma separator)" 
  gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/test-table-comma.csv" 
  options='{
    "separator":","
    "pagination":{
      "itemsPerPage":5
    },
    "cardsview": { "activate": true, "default": true },
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
```

### Don't panic!

Gitribute includes a button to copy-paste an existing widget in one click, so you won't have to write your whole widget from scratch.
