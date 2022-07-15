---
background-color: white
logo-left: https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/logo_GITRIBUTE_title_big.png
fixed-top: true

buttons-left-centered: true

buttons-left: 

  - name: the-gitribute-prject
    icon: help-circle
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
          en: Why Gitribute ?
      - name: features
        link: /main-features
        component: simpleLink
        label: 
          fr: Principales fonctionnalités
          en: Main features
      - name: sep
        separator: true
      - name: business-model
        link: /business-model
        component: simpleLink
        label: 
          fr: Quel est le business model ?
          en: What is the business model ?
      - name: benchmark
        link: /benchmark
        component: simpleLink
        label: 
          fr: Benchmark
          en: Benchmark

  - name: tutorials
    icon: school
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Tutoriels
      en: Tutorials
    submenu: 
      - name: integration
        link: /integration
        component: simpleLink
        label: 
          fr: Intégration
          en: Integration
      - name: sep
        separator: true
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
      - name: sep
        separator: true
      - name: quickstart-developpers
        link: /quickstart-developpers
        component: simpleLink
        label: 
          fr: Développeurs.euses
          en: Quickstart for developpers

  # - name: installation 
  #   icon: code-greater-than
  #   component: dropdownLink
  #   options: [ arrowless, hoverable ]
  #   label: 
  #     fr: Installation
  #     en: Installation
  #   submenu:
  #     - name: install
  #       link: /install
  #       component: simpleLink
  #       label: 
  #         fr: Installation strategies
  #         en: Installation strategies

  - name: documentation 
    icon: book-open-variant
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Documentation
      en: Documentation
    submenu:
      - name: install
        link: /install
        component: simpleLink
        label: 
          fr: Installation strategies
          en: Installation strategies
      - name: sep
        separator: true
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
          fr: Widget "gitfile"
          en: Widget "gitfile"
      - name: multi-files
        link: /docs-multi-files
        component: simpleLink
        label: 
          fr: Widget "multi-files"
          en: Widget "multi-files"
      - name: explowiki
        link: /docs-explowiki
        component: simpleLink
        label: 
          fr: Widget "explowiki"
          en: Widget "explowiki"
      - name: sep
        separator: true
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
          fr: Architecture & sketches
          en: Architecture & sketches
      - name: software
        link: /software
        component: simpleLink
        label: 
          fr: Software infos
          en: Software infos
      # - name: roadmap
      #   link: /roadmap
      #   component: simpleLink
      #   label: 
      #     fr: Feuille de route
      #     en: Roadmap

  - name: gallery
    disabled: false
    icon: image
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Galerie
      en: Gallery
    submenu:
      # - name: demo-cooptech
      #   link: /demo-cooptech
      #   component: simpleLink
      #   label: 
      #     fr: Cooptech - annuaire
      #     en: Cooptech - organisations
      # - name: sep
      #   separator: true
      # - name: demo-odf-observatoire
      #   link: /demo-odf-observatoire
      #   component: simpleLink
      #   label: 
      #     fr: Open Data France - Données de l'Observatoire
      #     en: Open Data France - Observatory's datasets
      # - name: demo-odf-ressources
      #   link: /demo-odf-ressources
      #   component: simpleLink
      #   label: 
      #     fr: Open Data France - Ressources
      #     en: Open Data France - Ressources
      # - name: sep
      #   separator: true
      # - name: demo-fabmob
      #   link: /demo-fabmob
      #   component: simpleLink
      #   label: 
      #     fr: Fabmob - Projets du wiki
      #     en: Fabmob - Projects from wikimedia
      # - name: demo-aac
      #   link: /demo-aac
      #   component: simpleLink
      #   label: 
      #     fr: AAC - Projets du wiki
      #     en: AAC - Projects from wikimedia

      - name: gitribute-cooptech
        link: /gitribute-cooptech
        component: simpleLink
        label: 
          fr: Cooptech - annuaire
          en: Cooptech - organisations
      - name: sep
        separator: true
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
      - name: sep
        separator: true
      - name: gitribute-explowiki-fabmob
        link: /gitribute-explowiki-fabmob
        component: simpleLink
        label: 
          fr: Fabmob - Projets du wiki
          en: Fabmob - Projects from wikimedia
      - name: demo-aac
        link: /demo-aac
        component: simpleLink
        label: 
          fr: AAC - Projets du wiki
          en: AAC - Projects from wikimedia

  - name: contact 
    icon: at
    link: /contact
    component: simpleLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Contact
      en: Contact

buttons-right: 

  - name: multi 
    link: https://multi.coop
    image: https://raw.githubusercontent.com/multi-coop/gitribute-documentation-content/main/images/logos/logo-multi-003.png
    icon: open-in-new
    component: extLink
    options: [ arrowless ]
    label: 
      fr: A project by the tech cooperative multi
      en: A project by the tech cooperative multi

  - name: repo 
    link: https://gitlab.com/multi-coop/gitribute
    icon: gitlab
    component: extLink
    options: [ arrowless ]
    label: 
      fr: Code source de Gitribute
      en: Gitribute source code

  - name: switch-locale
    component: switchLocaleDropdown
    options: [ arrowless, uppercase, rounded, hoverable ]


--- 

# Navbar config file
