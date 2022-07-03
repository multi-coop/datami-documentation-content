---
name: Data Patch

clients: 
  - Free
  - ADEME

period: 
  fr: avril-mai 2021

type:
  fr:
    - projet-indépendant
    - communs-numériques
    - open-data

description:
  fr: |
    Proposer une alternative à des éditeurs en ligne de bases de données propriétaires tels que Airtable, en y ajoutant une fonctionnalité de contribution ouverte / modération (s'inspirant de Wikipedia). 

    Faciliter la mise à jour de données par des communautés d'utilisateurs.

    Application sécurisée d'édition de données tabulaires, de partage de données (API, iframe, widget), de gestion de base de données relationnelles, de contribution ouverte et de modération.

approach:
  fr: 
    - tables postgreSQL générées à la volée
    - backend indépendant et générique d'API-fication
    - frontend indépendant
    - multilingue / responsive

resources:
  fr: 
    - 1 développeur fullstack
    - 1 product owner

technos: [ Javascript, Vue.js, Nuxt.js, Draggable.js, PostgreSQL, Oauth2, FastAPI, SocketIO, Y.js, i18n ]

refs:
  - name: ademe
    link: https://wiki.resilience-territoire.ademe.fr/wiki/Data_Patch
    fr: Documentation sur le wiki Résilience des Territoires
  - name: tipee
    link: https://fr.tipeee.com/data-patch/
    fr: Page Tipee
  - name: anct
    link: https://mon.incubateur.anct.gouv.fr/processes/transformation-numerique/f/5/proposals/242
    fr: Proposition sur le site de consultation de l'ANCT

code:
  - name: front
    link: https://github.com/co-demos/datapatch-front
    fr: frontend
  - name: back
    link: https://github.com/co-demos/fastapi-boilerplate
    fr: Backend

cover: ./images/references/data-patch/data-patch-logo.png

images:
  - ./images/references/data-patch/datapatch-01.png
  - ./images/references/data-patch/datapatch-02.png
  - ./images/references/data-patch/datapatch-03.png
  - ./images/references/data-patch/datapatch-04.png

---
