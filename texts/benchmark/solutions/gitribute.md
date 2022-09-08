---
name: Datami

open: 
  - "yes"

stage: 
  - In development

period: 
  en: Since 2022 (développement continu)

type:
  en:
    - widget
    - générique 
    - open-data

description:
  en: |
    Outil générique de type widget, permettant de visualiser et d'éditer des données hébeergées sur Github ou Gitlab, voire sur un mediawiki.

    Datami possède différentes fonctionnalités visant à simplifier l'édition de données et leur enrichissement :

    - visualisation sous forme de tableau ou de tuiles
    - visualisation des différences entre la version originale et la version éditée par l'utilisateur
    - recherche par filtres ou en fulltext
    - import / export des données
    - consolidation de données par requête à des APIs externes
    - appliquer un schéma de données sur des données de type tableur
    - bouton pour copier/coller facilement le bloc html du widget
    - parcours simplifié permettant de créer une merge request
    - injection de données externes (référentiels, clé étrangères)

approach:
  en: 
    - 
    - outil générique de visualisation et d'édition de données
    - widget intégrable dans tout site web
    - accent mis sur la simplicité d'utilisation et l'UX 
    - responsive

technos: [
  Javascript,
  Vue.js,
  Bulma,
  Buefy,
  Git
]

code:
  - name: app
    link: https://gitlab.com/multi-coop/gitribute
    en: Source code
  - name: docs
    link: https://gitribute-docs.multi.coop/
    en: Documentation

images:
  - ./images/logo_GITRIBUTE.png
  - ./images/screenshots/multifiles-preview-01.png
  - ./images/screenshots/gitfile-md-preview-01.png
  - ./images/screenshots/gitfile-csv-preview-01.png
  - ./images/screenshots/gitfile-json-preview-01.png
  - ./images/screenshots/explowiki-preview-01.png


---
