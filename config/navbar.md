---
background-color: white
logo-left: ./images/logo_GITRIBUTE.png
fixed-top: true

buttons-left-centered: true

buttons-left: 

  - name: who-are-we 
    # link: /who-are-we
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
      - name: how-it-works
        link: /how-it-works
        component: simpleLink
        label: 
          fr: Comment ça marche ?
          en: How does it work ?
      - name: features
        link: /main-features
        component: simpleLink
        label: 
          fr: Principales fonctionnalités
          en: Main features
      - name: roadmap
        link: /roadmap
        component: simpleLink
        label: 
          fr: Feuille de route
          en: Roadmap
      # - name: references
      #   link: /references
      #   component: simpleLink
      #   label: 
      #     fr: Ils utilisent Gitribute 
      #     en: They use Gitribute
      # - name: team
      #   link: /team
      #   component: simpleLink
      #   label: 
      #     fr: Equipe
      #     en: Team
      - name: architecture
        link: /architecture
        component: simpleLink
        label: 
          fr: Architecture
          en: Architecture
      - name: stack
        link: /stack
        component: simpleLink
        label: 
          fr: Stack
          en: Stack

  - name: tutorials
    # link: /who-are-we
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
      - name: quickstart
        link: /quickstart
        component: simpleLink
        label: 
          fr: Installation rapide
          en: Quickstart
      - name: integration
        link: /integration
        component: simpleLink
        label: 
          fr: Intégration
          en: Integration
      - name: lookup
        link: /install
        component: simpleLink
        label: 
          fr: Installation strategies
          en: Installation strategies

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

  - name: contact 
    link: /contact
    component: simpleLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Contactez-nous
      en: Contact us

  # - name: blog
  #   link: /blog
  #   component: simpleLink
  #   label: 
  #     fr: Blog
  #     en: Blog

  - name: gallery
    disabled: false
    # link: /we-like
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Galerie
      en: Gallery
    submenu:
      # - name: network
      #   link: /network
      #   component: simpleLink
      #   label: 
      #     fr: Notre réseau
      #     en: Our network
      # - name: ressources
      #   link: /ressources
      #   component: simpleLink
      #   label: 
      #     fr: Ressources
      #     en: Ressources
      - name: odf-data
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: Open Data France - Données de l'Observatoire
          en: Open Data France - Observatory's datasets
      - name: odf-ressources
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: Open Data France - Ressources
          en: Open Data France - Ressources
      - name: fabmob-projects
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: Fabmob - Projets du wiki
          en: Fabmob - Projects from wikimedia
      - name: ademe-projects
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: ADEME - Projets du wiki
          en: ADEME - Projects from wikimedia
      - name: cooptech-registry
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: CoopTech - Annuaire descoopératives
          en: CoopTech - Cooperatives registry

  - name: switch-locale
    component: switchLocaleDropdown
    options: [ arrowless, uppercase, rounded, hoverable ]
    

--- 

# Navbar config file
