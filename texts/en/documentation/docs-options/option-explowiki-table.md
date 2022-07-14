
##### Keys for the `options` parameter for `mediawiki` data

```yaml
"options":
  - description : JSON object containing the options allowing your mediawiki ressources to be parsed correctly
  - type: object
  - required: true
  - default: {
      "wikisettings": {
        "category": "projet",
        "fields": [
          "url",
          "description",
          "shortDescription",
          "Main_Picture",
          "Tags"
        ],
        "tagfields": [
          "Tags"
        ]
      },
      "pagination": {
        "itemsPerPage":12
      },
      "pagination": {
        "itemsPerPage": 5
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
    }

  - fields:

    - "wikisettings"
      description: settings to retrieve and parse mediawiki ressources
      type: object
      fields:
        - "category"
          description: the name of the ressources' category to retrieve
          required: true
          type: string
        - "fields"
          description: list of fields you want to parse from the wikitext format
          required: true
          type: [ string ]
      - "tagfields"
          description: list of fields you want to parse as tags
          type: [ string ]

    - "pagination": 
      description: pagination settings
      type: object
      fields:
      - "itemsPerPage":
        description: number of items per page
        default: 20
        type: number
        notes: 
        - must be > 1 and within allowed values, or a default value will be used (the closest value from allowed values array)
        - values : [3, 5, 10, 15, 20, 25, 50, 100]

    - "cardsview":
      description: allows cards view on a table data
      type: boolean || object
      default: false
      notes: |
        You can pass an object instead of a boolean value if you need to display the cards view by default, with :
        { "activate": true, "default": true }

    - "cardsdetail":
      description: allows cards detailled view on a table data
      type: boolean
      default: false

    - "cardssettings":
      description: |
        Mandatory settings to display table data, field by field, in a card view. 
        You can chose to display data diffently between "mini" card view (tiles) and the "detailled" card view...
        For "mini" and "detail" entries you have to map a key from your original data (f.i. the "name" column) to a position in the cards (f.i. apply the "name" value to the "title")
      type: object
      default: {
        "mini": {
          "<KEY-COLUMN>": {"position": "<POSITION-IN-CARD>"},
          ...
        },
        "detail": {
          "<KEY-COLUMN>": {"position": "<POSITION-IN-CARD>"},
          ...
        }
      }
      notes: The possible positions in cards are for now te following :
        - "title"
        - "subtitle"
        - "content"
        - "resume"
        - "description"
        - "image" (needs an url to an image)
```
