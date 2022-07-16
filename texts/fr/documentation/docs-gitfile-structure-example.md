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
```
