
## How to integrate the Gitribute widgets

Widgets need two files in order to work :

- `app.js`
- `app.css`

Add those two files to your html head, like this if the widget code is deployed on `https://gitribute.multi.coop`:

```html
<script src="https://gitribute.multi.coop/js/app.js" type="text/javascript"></script>

<link type="text/css" href="ttps://gitribute.multi.coop/js/app.css" rel="stylesheet">
```

Widgets can then be called directly into the page as custom html elements.
