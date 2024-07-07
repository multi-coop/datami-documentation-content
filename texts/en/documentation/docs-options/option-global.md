
### The `options` parameter

A widget can take several optional parameters, some of them depending on your input file's type (`csv`, `json`, `md`, ...) and on the widget you use (`datami-gitfile`, `datami-explowiki`, `datami-multi-files`)

---

#### Structure

```yaml
"options":
  - description : The options object contains all specifics setup for your particular widget
  - required: false
  - type: object
  - default: {}
```

---

#### Options keys
