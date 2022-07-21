## Preuve de concept (POC) 

**Développements : avril-juillet 2022**

La première étape du projet était de prouver que le concept et les hypothèses de départ étaient transposables et faisables techniquement.

Nous avions besoin d'être certains des choses suivantes :

- Savoir utiliser les APIs de Github et Gitlab via des fonctions communes ;
- Être capables de mettre en place des widgets / composants web correctement...
- ... avec un _framework_ que l'équipe de développement maîtrise ;
- Pouvoir faire les premiers développements dans le cadre de missions pour des **vrais** clients et de **vrais** besoins ;
- _[Do it agile or do not, there is no try](https://www.youtube.com/watch?v=BQ4yd2W50No)..._

### Notre liste de courses pour une recette de joli POC

Notre **feuille de route** pour la preuve de concept (POC) était la suivante :

- [x] Un squelette de widget avec `vue-custom-element` / `vuejs` : vuex, dépendances, _linting_, ... ;
- [x] Premières fonctions de base utilitaires et _mixins_ pour manipuler les données d'un fichier hébergé sur Gitlab/Github ;
  - [x] Récupérer des infos à partir de l'URL du fichier : repo, orga, branche, type de fichier... ;
  - [x] Récupérer les données brutes ("raw") depuis le service Git ;
  - [x] Formatter les données brutes dans un format attendu pour le type de fichier (`md`, `csv`, `json`, `mediawiki` > objets) ;
- [x] Installer un framework CSS pour Vuejs ( Bulma + Buefy ) ;
- [x] Préparet une solution _custom_ d'internationalisation (i18n ne s'est pas révélé super adapté dans notre cas);
- [x] Créer les premiers composants principaux :
  - [x] Créer un squelette d'affichage pour chacun des types de fichiers utiles ;
  - [x] Prévisualisation d'un fichier `.md` ;
  - [x] Prévisualisation d'un fichier `.csv` ;
  - [x] Prévisualisation d'un fichier `.json` ou `.geojson` ;
  - [x] Prévisualisation d'une liste de ressources provenant d'un `mediawiki`, convertie en pseudo-table ;
  - [x] Composant permettant de mettre à jour le _token_ utilisateur (si l'utilisateur en a un et souhaite faire des commits directs sur la branche mère) ;
  - [x] Composant pour alterner entre les traductions, pour le moment entre `français` et `anglais` ;
- [x] Créer un "utilisateur fantôme" sur Gitlab et un autre sur Github pour faire des tests, et permettant d'opérer des modifications anonymement (en utilisant le _token_ fantôme dans le widget) ;
- [x] Autre composants principaux :
  - [x] Pour chacun des types de fichiers, alterner entre vues 'prévisualisation', 'diff', et 'édition' ;
    - [x] pour les fichiers `csv` (`.csv` et `.tsv`)
    - [x] pour les fichiers `text` (`.md`)
    - [x] pour les fichiers `json` (`.json` et `.geojson`)
    - [x] pour les ressources `mediwiki` (seulement en `preview` pour le moment)
  - [x]  Ajouter un bouton `Upload` + dialogue + actions pour écraser les données du widget ;
  - [x]  Ajouter in paramètres `lockHeaders` dans les options pour protéger les champs en édition ;
  - [x]  Ajouter un bouton `Sauver` + dialogue + actions :
    - [x] `POST` pour créer une branche séparée sur le repo du fichier source ;
    - [x] `PUT` après l'édition côté client, pour faire des commits sur la nouvelle branche créée ;
    - [x] Créer une `merge request` (commit + request faites par défaut par l'utilisateur fantôome) ; 
- [x] Déployer sur Netlify pour les tests et la production => [url de déploiement de prod](https://gitribute.multi.coop/)
  - [![Netlify Status](https://api.netlify.com/api/v1/badges/1cd66edf-3b08-43db-bd21-6490377bb24a/deploy-status)](https://app.netlify.com/sites/multi-gitribute/deploys)
- [ ] Une documentation la plus complète possible pour le projet et chacun des widgets **<--- On en est là, plus qu'une case à cocher !!**

... et pour ce qui est du POC, [that would be greaaaaat... mmm'kay ?](https://www.youtube.com/watch?v=JFRa7Ovym8s&ab_channel=IAJSTU)

**Work in progress... la fin est prooooche (hésitez pas si vous voulez filer un coup de main) :)**
