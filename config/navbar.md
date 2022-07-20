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
      - name: business-model
        link: /business-model
        component: simpleLink
        label: 
          fr: "100% libre & gratuit"
          en: "100% free"
      - name: features
        link: /main-features
        component: simpleLink
        label: 
          fr: Principales fonctionnalités
          en: Main features
      - name: sep
        separator: true
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
      - name: tutorial-overview
        link: /tutorial-overview
        component: simpleLink
        label: 
          fr: Panorama des tutoriels
          en: Overview
      - name: sep
        separator: true
      - name: tutorial-actions
        link: /tutorial-actions
        component: simpleLink
        label: 
          fr: Actions
          en: Actions
      - name: tutorial-views
        link: /tutorial-views
        component: simpleLink
        label: 
          fr: Vues
          en: Views
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
      - name: integration
        link: /integration
        component: simpleLink
        label: 
          fr: Intégration
          en: Integration
      - name: integration-wordpress
        link: /integration-wordpress
        component: simpleLink
        label: 
          fr: Intégration Wordpress
          en: Wordpress integration

  - name: documentation 
    icon: book-open-variant
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Documentation
      en: Documentation
    submenu:
      - name: docs-widgets-overview
        link: /docs-widgets-overview
        component: simpleLink
        label: 
          fr: Panorama des widgets
          en: Widgets overview
      - name: sep
        separator: true
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
      - name: install
        link: /install
        component: simpleLink
        label: 
          fr: Stratégies d'installation
          en: Installation strategies
      - name: quickstart-developpers
        link: /quickstart-developpers
        component: simpleLink
        label: 
          fr: Développeurs.euses
          en: Quickstart for developpers
      - name: sep
        separator: true
      - name: software
        link: /software
        component: simpleLink
        label: 
          fr: Infos sur le logiciel
          en: Software infos

  - name: gallery
    disabled: false
    icon: image
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Exemples
      en: Examples
    submenu:
      - name: demo-cooptech
        link: /demo-cooptech
        component: simpleLink
        label: 
          fr: Cooptech - annuaire
          en: Cooptech - organisations
      - name: sep
        separator: true
      - name: demo-odf-observatoire
        link: /demo-odf-observatoire
        component: simpleLink
        label: 
          fr: Open Data France - Données de l'Observatoire
          en: Open Data France - Observatory's datasets
      - name: demo-odf-ressources
        link: /demo-odf-ressources
        component: simpleLink
        label: 
          fr: Open Data France - Ressources
          en: Open Data France - Ressources
      - name: sep
        separator: true
      - name: demo-fabmob
        link: /demo-fabmob
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

      # - name: gitribute-cooptech
      #   link: /gitribute-cooptech
      #   component: simpleLink
      #   label: 
      #     fr: Cooptech - annuaire
      #     en: Cooptech - organisations
      # - name: sep
      #   separator: true
      # - name: gitribute-odf-observatoire
      #   link: /gitribute-odf-observatoire
      #   component: simpleLink
      #   label: 
      #     fr: Open Data France - Données de l'Observatoire
      #     en: Open Data France - Observatory's datasets
      # - name: gitribute-odf-ressources
      #   link: /gitribute-odf-ressources
      #   component: simpleLink
      #   label: 
      #     fr: Open Data France - Ressources
      #     en: Open Data France - Ressources
      # - name: sep
      #   separator: true
      # - name: gitribute-explowiki-fabmob
      #   link: /gitribute-explowiki-fabmob
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
      fr: Un projet par la coopérative multi
      en: A project by the tech cooperative multi

  - name: blog 
    # icon: at
    link: /blog
    component: simpleLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Blog
      en: Blog

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
