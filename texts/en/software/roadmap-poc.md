## Proof Of Concept (POC) 

**Developments : april-july 2022**

The first step of the project was to prove our ideas and hypothesis were technically working.

We needed to be sure :

- To know how to use Github and Gitlab APIs with common functions ;
- To be able to setup working widgets...
- ... in a frameworks we understood amongst the team ;
- Do all those early developments with **real** users and clients ;
- _[Do it agile or do not, there is no try](https://www.youtube.com/watch?v=BQ4yd2W50No)..._

### Our to-do list for a nice POC

The **roadmap** for a first proof of concept (POC) was the following :

- [x] Skeleton for `vue-custom-element` / `vuejs` : vuex (shared store between all web components), dependencies, linting, ... ;
- [x] First utils functions and mixins to process a file's gitlab/github url ;
  - [x] Get all git infos from file's url ;
  - [x] Get file's raw data from provider ;
  - [x] Format file's raw data to expected structures (from `md`, `csv`, `json`, `mediawiki` to objects) ;
- [x] Install a CSS framework for Vuejs ( Bulma + Buefy ) ;
- [x] Prepare a simple multi-language / translation solution (i18n not adapted for our purposes);
- [x] Create the first main components :
  - [x] For each file type create a loading skeleton while waiting raw file to finish loading ;
  - [x] Preview for a `.md` file ;
  - [x] Preview for a `.csv` file ;
  - [x] Preview for a `.json` or `.geojson` file ;
  - [x] Preview for a list of `mediawiki` ressources, converted as pseudo-table ;
  - [x] Component to update user's token (if user has a specific one for direct commits) ;
  - [x] Component to switch between `french` and `english` for now ;
- [x] Create a "ghost user" on gitlab and github for test purposes, acting as anonymous gitlab/github users (with their token, injected in web component) ;
- [x] Other main components :
  - [x] On each preview (for every file type), switch between 'preview' and 'edition' views ;
    - [x] for `csv` files (`.csv` and `.tsv` types)
    - [x] for `text` files (`.md` types)
    - [x] for `json` files (`.json` and `.geojson` types)
    - [x] for `mediwiki` ressources (only preview for now)
  - [x]  Add an `Upload` button + dialog + actions to overwrite whole edited data ;
  - [x]  Add a `lockHeaders` options in widget to only protect keys from edition ;
  - [x]  Add a `Save` button + dialog + actions :
    - [x] `POST` create a separate branch on the file's repo ;
    - [x] `PUT` after edition on client's side, acting as a commit to the file's git repo on a separate branch ;
    - [x] create a merge request (commit and request by default done the "ghost user") ; 
- [x] Deploy on Netlify for tests and production purposes => [deploy here](https://gitribute.multi.coop/)
  - [![Netlify Status](https://api.netlify.com/api/v1/badges/1cd66edf-3b08-43db-bd21-6490377bb24a/deploy-status)](https://app.netlify.com/sites/multi-gitribute/deploys)
- [ ] A good documentation for each web component (at least in this readme for now) **<--- We are here, we just have one checkbox left !!**

... and just for a POC, [that would be greaaaaat... mmm'kay ?](https://www.youtube.com/watch?v=JFRa7Ovym8s&ab_channel=IAJSTU)

**Work in progress... the end is near (or help us by contributing) :)**
