
## How to integrate your customized Gitribute widgets

### Dependencies

Gitribute's widgets need several files and the widget's block in order to work correctly :

- `app.js` : the Gitribute application itself
- `app.css` : Gitribute's styles
- `materialdesignicons-webfont.woff2`: : Gitribute's icons
- and finally the widget's `html` block (`<multi-gitribute-file>`, `<multi-gitribute-multi-files>`, ...)

The `css` and `font` files are imported automatically, you just have to add the script and the widget's block to integrate a widget to your page.

### Integration examples

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

### Don't panic !

Gitribute includes **a button to copy an existing widget in one click**, so you won't have to write your whole widget from scratch.

Once clicked, **you just have to paste it in a web page** of you choice !

> **Note** : More details about the widgets action buttons in the ["Tutorials > Actions"](/tutorial-actions) section.
