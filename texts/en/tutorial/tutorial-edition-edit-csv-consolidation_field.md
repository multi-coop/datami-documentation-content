### Consolidation field

<div>
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate.png"
    />
</div>

With Gitribute you can add a customized "consolidation field" to request external APIs, in order to delegate some refinement operations to external services.

Each API could be configured independantly.

Once consolidation is configured for a particular table file, a Gitribute widget will display a "consolidation" column (or `field`) on the left side of the table.

For each row this consolidation field will display a consolidation button. 

By clicking on this button the user will or could have several consolidation APIs to chose from.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE-ROW"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate-row.png"
    />
</div>

<br>

When you click on one of the consolidation services listed, a request is sent to the API and if the external API returns any result you will see a drawer appearing below your row.

<div style="border: thin solid lightgrey;">
  <img
    alt="TUTORIAL-EDITION-CSV-CONSOLIDATE-ROW"
    src="https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/tutorial/edit-csv/edit-csv-consolidate-row-result.png"
    />
</div>

<br>

This drawer contains the "old" and "new" values : "old" being the value inside your row, new being the value returned by the API.

To overwrite the "old" value by the "new" one, just select the field(s) you want to overwrite and click on "Validate the changes".

> **Note** : More about how to add consolidation properties to a table dataset, with the Gitribute `gitfile` widget, in the **["Documentation > Widget 'gitfile'"](/docs-gitfile)** section.
