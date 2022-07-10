### Data consolidation

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

> **Note** : More on the consolidation in the **["Tutorial > Edition"](/tutorial-edition)** section
