### Table fields

To be a bit more accurate we will use the terme `field` instead of `column` in this section.

The fields are listed horizontally in the first row, as they are written in the source file.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELDS"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-fields.png"
    />
</div>

<br>

If configured as such in the widget's options a field could be locked to prohibit any modification.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELD-LOCKED"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-field-locked.png"
    />
</div>

<br>

#### Table fields, table schema, and table properties

With Gitribute you can apply a [table schema](https://specs.frictionlessdata.io/table-schema/) and other properties to a raw `csv` file.

You can have a look of a field's properties just by hovering it.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELD-TOOLTIP"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-field.png"
    />
</div>

<br>

Those properties can either be "hard-coded" in the widget's html block, or they can be stored externally in third-party files.

A field's property contains informations like :

- The field's **name** ;
- The field's **description** ;
- The field's **type** : `string`, `boolean`, `number`, ... ;
- And many others informations helping in displaying the data the more accuratly as possible ;

Those informations constitues a "table schema".

For table schema we use the [`Table Schema` standard](https://specs.frictionlessdata.io/table-schema/), described there in the [Frictionless data website](https://specs.frictionlessdata.io).

In addition to the Table Schema standard Gitribute uses other informations to describe a field, in order to optimize the user experience. Those extra informations are what we call the file's "custom properties".

If the schema or the properties are described in external files you can check those files directly from the file's info dialog (by clicking on the <span class="icon"><i class="mdi mdi-information-outline"></i></span> button).

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-FIELDS"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-schema_props.png"
    />
</div>

<br>

> More about how to apply a schema and properties to a table dataset with Gitribute `gitfile` widget in the **["Documentation > Widget 'gitfile'"](/docs-gitfile)** section.
