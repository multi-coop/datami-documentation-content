
## Roadmap

**Work in progress... be patient guys (or help us by contributing) :)**

This project is currently under early development...

The **roadmap** for a first proof of concept (POC) is the following :

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
- [x] Deploy on Netlify for test purposes => [test deploy here](https://multi-gitribute-test.netlify.app/)
- [ ] A good documentation for each web component (at least in this readme for now)

... and just for a POC, that would be greaaaaat ...
