
##### Keys for the `options` parameter for the `multi-files` widget

```yaml
"options":
  - description : JSON object containing the options for multifiles
  - type: object
  - required: true
  - default: {
      "display": "horizontal"
    }
  
  - fields: 

    - "display": 
      description: default display of your multi-files tabs
      type: string
      allowed values: [ "horizontal", "vertical" ]
```
