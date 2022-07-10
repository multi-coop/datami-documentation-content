---
background-color: white
logo-left: https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/logo_GITRIBUTE_title_big.png
fixed-top: true

buttons-left-centered: true

buttons-left: 

  - name: the-gitribute-prject
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Pourquoi Gitribute ?
      en: Why Gitribute
    submenu: 
      - name: why-gitribute
        link: /why-gitribute
        component: simpleLink
        label: 
          fr: Pourquoi Gitribute ?
          en: Why Gitribute
      - name: features
        link: /main-features
        component: simpleLink
        label: 
          fr: Principales fonctionnalités
          en: Main features
      - name: how-it-works
        link: /how-it-works
        component: simpleLink
        label: 
          fr: Comment ça marche ?
          en: How does it work ?
      - name: architecture
        link: /architecture
        component: simpleLink
        label: 
          fr: Architecture
          en: Architecture
      - name: roadmap
        link: /roadmap
        component: simpleLink
        label: 
          fr: Feuille de route
          en: Roadmap
      - name: benchmark
        link: /benchmark
        component: simpleLink
        label: 
          fr: Benchmark
          en: Benchmark

  - name: tutorials
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Tutoriels
      en: Tutorials
    submenu: 
      - name: tutorial-overview
        link: /tutorial-overview
        component: simpleLink
        label: 
          fr: Overview
          en: Overview
      - name: tutorial-actions
        link: /tutorial-actions
        component: simpleLink
        label: 
          fr: Actions
          en: Actions
      - name: tutorial-edition
        link: /tutorial-edition
        component: simpleLink
        label: 
          fr: Edition
          en: Edition
      - name: tutorial-contribution
        link: /tutorial-contribution
        component: simpleLink
        label: 
          fr: Contribution
          en: Contribution

  - name: installation 
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Installation
      en: Installation
    submenu:
      - name: lookup
        link: /install
        component: simpleLink
        label: 
          fr: Installation strategies
          en: Installation strategies
      - name: integration
        link: /integration
        component: simpleLink
        label: 
          fr: Intégration
          en: Integration
      - name: quickstart-developpers
        link: /quickstart-developpers
        component: simpleLink
        label: 
          fr: Développeurs.euses
          en: Quickstart for developpers
      - name: stack
        link: /stack
        component: simpleLink
        label: 
          fr: Stack
          en: Stack

  - name: widgets 
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Widgets
      en: Widgets
    submenu:
      - name: docs-widgets-overview
        link: /docs-widgets-overview
        component: simpleLink
        label: 
          fr: Overview
          en: Overview
      - name: gitribute-file
        link: /docs-gitfile
        component: simpleLink
        label: 
          fr: gitribute-file
          en: gitribute-file
      - name: explowiki
        link: /docs-explowiki
        component: simpleLink
        label: 
          fr: gitribute-explowiki
          en: gitribute-explowiki
      - name: multi-files
        link: /docs-multi-files
        component: simpleLink
        label: 
          fr: gitribute-multi-files
          en: gitribute-multi-files
  

buttons-right: 

  - name: repo 
    link: https://gitlab.com/multi-coop/gitribute
    icon: gitlab
    component: extLink
    options: [ arrowless ]
    label: 
      fr: Code source de Gitribute
      en: Gitribute source code
  - name: contact 
    link: /contact
    component: simpleLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Contactez-nous
      en: Contact us

  - name: gallery
    disabled: false
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Galerie
      en: Gallery
    submenu:
      - name: gitribute-odf-observatoire
        link: /gitribute-odf-observatoire
        component: simpleLink
        label: 
          fr: Open Data France - Données de l'Observatoire
          en: Open Data France - Observatory's datasets
      - name: gitribute-odf-ressources
        link: /gitribute-odf-ressources
        component: simpleLink
        label: 
          fr: Open Data France - Ressources
          en: Open Data France - Ressources
      - name: gitribute-explowiki-fabmob
        link: /gitribute-explowiki-fabmob
        component: simpleLink
        label: 
          fr: Fabmob - Projets du wiki
          en: Fabmob - Projects from wikimedia
      - name: cooptech-registry
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: CoopTech - Annuaire des coopératives
          en: CoopTech - Cooperatives registry

  - name: switch-locale
    component: switchLocaleDropdown
    options: [ arrowless, uppercase, rounded, hoverable ]
    

--- 

# Navbar config file
