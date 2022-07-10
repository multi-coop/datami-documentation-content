
## To plead for quality data

Anybody who received table data (a spreadsheet, a csv) in its mail knows the challenges in reusing or even understanding table data you didn't produced yourself.

The data could come as either incomplete, not structured, some columns could be missing, some entries do not respect a referential, you'd need to geolocate your rows, etc... As delivered that kind of dataset is not "clean" nor ready for further uses.

**With Gitribute we try to adress this need for data consolidation**, mainly because that case is happening to uus daily at work with evrey client we work for : people's table data can always be "cleaner" or "better". To do so we mobilize two different families of tools : **schemas**, and **third party APIs**.

### Table data & schemas

"_Schemas_" are a key stone to make open data more interoperable. To help public or private actors making their open data more reusable and more valueable, **sharing common referentials is vital**.

Gitribute follows the trend of "[frictionless data](https://frictionlessdata.io/)" and some widgets allow to **[apply table schema](/docs-gitfile)** to the tables you share in a widget.

The French State has a strong roadmap regarding schemas, and there is already a good [list of schemas already existing](https://schema.data.gouv.fr/schemas.html) to create or analyze datasets.

Our intention with Gitribute is to allow actors with more modest means than a state (!) or big companies to use schemas. If schemas are vital to make better open data, and if we want common citizen to produce open data, **using a schema upon table data should be trivial or transparent**.

### Table data consolidation

We encounter multiple use cases where we needed to "consolidate" a dataset by either changing/adding inputs inside the data, or by checking if data is how it is supposed to be like. 

"_Consolidating_" - in a broad understanding - means you need modifying your data to make it "cleaner" or "better", for instance :

- [Geolocate an adress](https://adresse.data.gouv.fr/csv) ; 
- [Validate your dataset respects a schema](https://validata.fr/) ; 
- [Generate an UUID](https://heidi.etalab.studio) ;
- [Retrieve public informations about a society](https://api.gouv.fr/les-api/api-entreprise)
- ... or [muuuuch more use cases](https://api.gouv.fr/).

Consolidation could concern either some rows only within a table, or also could concern the whole dataset. Finally consolidation needs on a dataset are usually related to a profession, a theme, a collective... Cases and combinations are infinite.

Given the infinite possible ways an user could need consolidation, our intention with Gitribute is to integrate but **delegate the consolidation to external services** (mostly third party APIs).

To keep helping users to benefit easily from those third party services, we though of a system to configure customized requests to APIs you'd need on a particular dataset. **Gitribute let the user chose which API they want to include given the specificities of a particular table**.

The integration of an **external API consolidation services is not hard-coded in Gitribute**, a Gitrbute widget only needs a setup in its **configuration file** for the consolidation button.

We already tested the integration of the following external APis into Gitribute :

- [API-entreprises](https://api.gouv.fr/les-api/api-entreprise) : helps retrieve public information about an entreprise or a public structure, given its SIREN number ;
- [Base Adresse Nationale](https://adresse.data.gouv.fr/api-doc/adresse) : helps geolocate an entity given a french postal adress in full text ;
- ... and much more to come.

More on the consolidation in the **["Tutorial > Edition"](/tutorial-edition)** section
