
## The widget `<multi-gitribute-file>`


This widget allows to preview and edit a file stored on Gitlab or Github.

---

### HTML tag

`<multi-gitribute-file/>`

---

### Screenshot

---

### Structure

The widget takes several parameters, following this structure :

```html
  <multi-gitribute-file 
    title='<YOUR-WIDGET-TITLE>'
    gitfile='<YOUR-FILE-URL-IN-GITLAB-OR-GITHUB>'
    options='{ <YOUR-OPTIONS> }'
    usertoken='<YOUR-USER-TOKEN or GHOST-USER-TOKEN>'
    locale='<YOUR-DEFAULT-LANGUAGE>'
  ></multi-gitribute-file>
```

---

### Example

```html
  <!-- Example for loading and contribute to a distant .csv file from Github -->
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

---

### Widget's parameters

This widget can take several parameters, some of them depends on your input file's type (`csv`, `json`, `md`, ...)
