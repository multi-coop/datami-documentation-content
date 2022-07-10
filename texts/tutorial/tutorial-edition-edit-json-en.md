## Edit a JSON file

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-JSON"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edition-edit-json.png"
    />
</div>

<br> 

Gitribute's `gitfile` widget can also edit `json` files (and it goes without saying also `geojson`).

You will have the exact same "edit-views" available for `json` files than for `md` or `csv` : `preview` / `edit` / `diff`.

A json object is displayed as "nodes" you can fold or open.

A json have a "root" level. At the `root` level you can find a `node` or an array.

A `node` can contain different types of items :

- Another node ;
- An object : `string`, `number`, `object`, `boolean` ;
- An array of nodes or objects. If so the name of the `node` is the `node`'s index in the array.

The `node`'s type is symbolized by a little red icon after its name :

- `{}` : `object`
- `[]` : `array`
- `abc` : `string`
- `123` : `number` or `float`
- `☑️` : `boolean`

In edition mode you can : 

- Add a new `node`, by clicking on the `+` icon.
- Remove a `node`, by clicking on the `trash` icon.
- Modify a `node` :
  - Change the `node`'s "key" if the `node` is an object, by clicking on the `pen` icon.
  - Change the `node`'s value

All of that recursively...

> **Note** :
>
> Json files are quite useful to describe unstructured informations, but there is also ways to validate a json file given a schema. 
>
> At the tech cooperative [multi](https://multi.coop) we are currently working on a [json validator](https://git.opendatafrance.net/outillages/json-validator) you would be interested in if you read this documentation until this section.
>
> From a nerd to a nerd, you know...
