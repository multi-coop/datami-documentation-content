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
      - name: What Gitribute does
        link: /what-gitribute-does
        component: simpleLink
        label: 
          fr: Principales fonctionnalités
          en: Main features
      - name: why-gitribute
        link: /why-gitribute
        component: simpleLink
        label: 
          fr: Pourquoi Gitribute ?
          en: Why Gitribute
      - name: references
        link: /references
        component: simpleLink
        label: 
          fr: Nos références
          en: Our references
      - name: team
        link: /team
        component: simpleLink
        label: 
          fr: Equipe
          en: Team

  - name: documentation 
    component: dropdownLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Documentation
      en: Documentation
    submenu:
      - name: lookup
        link: /documentation
        component: simpleLink
        label: 
          fr: Vue générale
          en: Global lookup
      - name: stack
        link: /documentation
        component: simpleLink
        label: 
          fr: Stack
          en: Stack
      - name: gitfile
        link: /documentation
        component: simpleLink
        label: 
          fr: Widget - gitfile
          en: Widget - gitfile
      - name: explowiki
        link: /documentation
        component: simpleLink
        label: 
          fr: Widget - explowiki
          en: Widget - explowiki
      - name: multi-files
        link: /documentation
        component: simpleLink
        label: 
          fr: Widget - multi-files
          en: Widget - multi-files
  
  - name: contact 
    link: /infos
    component: simpleLink
    options: [ arrowless, hoverable ]
    label: 
      fr: Contactez-nous
      en: Contact us

buttons-right: 

  - name: blog
    link: /blog
    component: simpleLink
    label: 
      fr: Blog
      en: Blog

  - name: examples
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
        link: /shares-simulator
        component: simpleLink
        label: 
          fr: Open Data France - Données de l'Observatoire
          en: Open Data France - Observatory's datasets
      - name: odf-ressources
        link: /shares-simulator
        component: simpleLink
        label: 
          fr: Open Data France - Ressources
          en: Open Data France - Ressources
      - name: fabmob-projects
        link: /shares-simulator
        component: simpleLink
        label: 
          fr: Fabmob - Projets du wiki
          en: Fabmob - Projects from wikimedia
      - name: ademe-projects
        link: /shares-simulator
        component: simpleLink
        label: 
          fr: ADEME - Projets du wiki
          en: ADEME - Projects from wikimedia
      - name: cooptech-registry
        link: /shares-simulator
        component: simpleLink
        label: 
          fr: CoopTech - Annuaire descoopératives
          en: CoopTech - Cooperatives registry

  - name: switch-locale
    component: switchLocaleDropdown
    options: [ arrowless, uppercase, rounded, hoverable ]
    

--- 

# Navbar config file
