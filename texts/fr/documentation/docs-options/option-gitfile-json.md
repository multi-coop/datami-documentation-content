
##### Keys for the `options` parameter for `json` and `geojson` files

```yaml
"options":
  - description : JSON object containing the options allowing your json to be parsed correctly
  - type: object
  - required: false
  - default: {
      "defaultDepth": 3,
    }

  - fields: 

    - "defaultDepth": 
      description: default visible depth of the JSON preview
      type: number | "all"

    - "allowKeyEdit": 
      description: allow objects' key edition (edit or remove)
      type: boolean
```
