---
routes: 

  # LANDING
  - name: home
    url: /
    # options:
    #   hero: true
    sections:
      - name: logo
        component: TextComponent
        options:
          columns-size: '5'
        files:
          fr: ./texts/landing/logo-gitribute.md
          en: ./texts/landing/logo-gitribute.md
      - name: catchphrase
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/landing/catchphrase-en.md
          en: ./texts/landing/catchphrase-en.md
      - name: btns
        component: ButtonsComponent
        options:
          columns-size: three-quarters
          buttons-size: one-third
          buttons:
            - link: /tutorial-overview
              icon-left: school
              rounded: true
              label: 
                fr: Tutorials
                en: Tutorials
            - link: /why-gitribute
              icon-left: help-circle
              rounded: true
              label:
                fr: Pourquoi Gitribute ?
                en: Why Gitribute ?
            - link: /docs-widgets-overview
              icon-left: book-open-variant
              rounded: true
              label: 
                fr: Doc des widgets
                en: Widgets' docs
            # - link: https://gitlab.com/multi-coop/gitribute
            #  icon-left: gitlab
            #  rounded: true
            #  label: 
            #    fr: Code source
            #    en: Source code
      - name: more
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/landing/more.md
          en: ./texts/landing/more.md
      # - name: intro-widget
      #   component: HtmlComponent
      #   options:
      #     columns-size: two-thirds
      #   files:
      #     fr: ./texts/landing/landing-widget.html
      #     en: ./texts/landing/landing-widget.html
      - name: intro
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/landing/landing-intro-en.md
          en: ./texts/landing/landing-intro-en.md
      - name: more-1
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/landing/more.md
          en: ./texts/landing/more.md
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: two-thirds
          js: 
            - href: https://gitribute.multi.coop/js/app.js
          css: 
            - href: https://gitribute.multi.coop/css/app.css
          html: |
            <multi-gitribute-file
              title="Liste des coopératives de la tech en France - csv ( semicolon separator)"
              gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/cooptech/Annuaire-SCOP-SCIC-tech-France.csv"
              options='{
                "height": "500px",
                "separator":",",
                "lockcolumns": true,
                "tagseparator":",",
                "customfilters" : {
                  "activate": true,
                  "filterfields": [
                  "type",
                    "Statut juridique"
                    ]
                },
                "schema": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-schema.json"
                },
                "fields-custom-properties": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-fields-custom-props.json"
                },
                "customsorting" : {
                  "activate": true,
                  "sortfields": [
                    { "name": "Nom" }
                  ]
                },
                "pagination":{
                  "itemsPerPage": 20
                },
                "cardsview": {
                  "activate": true,
                  "default": false
                },
                "cardsdetail": true,
                "cardssettings": {
                  "mini": {
                    "Nom": {"position": "title"},
                    "Présentation": {"position": "description"},
                    "Site internet": {"position": "description"},
                    "Statut juridique": {"position": "tags"},
                    "Domaine(s)": {"position": "tags"}
                  },
                  "detail": {
                    "Nom": {"position": "title"},
                    "Site internet": {"position": "description"},
                    "Présentation": {"position": "description"},
                    "Numéro SIREN": {"position": "description"},
                    "Adresse": {"position": "description"},
                    "Statut juridique": {"position": "tags"},
                    "Domaine(s)": {"position": "tags"},
                    "Fiche URSCOP": {"position": "links"}
                  }
                }
              }'
              usertoken=""
              locale="fr"
              debug="false"
            />
      - name: more-2
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/landing/more.md
          en: ./texts/landing/more.md
      - name: outro
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/landing/landing-outro-en.md
          en: ./texts/landing/landing-outro-en.md
      - name: more-3
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/landing/more.md
          en: ./texts/landing/more.md
      - name: clients
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/landing/landing-clients.md
          en: ./texts/landing/landing-clients.md
      - name: more-4
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/landing/more.md
          en: ./texts/landing/more.md
      - name: btn-to-why
        component: ButtonsComponent
        options:
          columns-size: three-quarters
          buttons-size: one-third
          buttons:
            - link: /why-gitribute
              icon-left: help-circle
              rounded: true
              label: 
                fr: Pourquoi Gitribute ?
                en: Why Gitribute ?
  
  # WHAT IS GITRIBUTE
  - name: why-gitribute
    url: /why-gitribute
    options:
      summary: true
      contrib: true
      name:
        en: Why Gitribute ?
    sections: 
      - name: why-intro
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/why-gitribute/why-gitribute-en.md
          en: ./texts/why-gitribute/why-gitribute-en.md
      - name: why-intro-easy
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Make open contribution easier 
        files:
          fr: ./texts/why-gitribute/why-gitribute-easy-en.md
          en: ./texts/why-gitribute/why-gitribute-easy-en.md
      - name: why-open
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Help organizations opening data
        files:
          fr: ./texts/why-gitribute/why-gitribute-open-en.md
          en: ./texts/why-gitribute/why-gitribute-open-en.md
      - name: why-costs
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Reduce the cost of open data
        files:
          fr: ./texts/why-gitribute/why-gitribute-costs-en.md
          en: ./texts/why-gitribute/why-gitribute-costs-en.md
      - name: why-quality
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Make quality open data
        files:
          fr: ./texts/why-gitribute/why-gitribute-quality-en.md
          en: ./texts/why-gitribute/why-gitribute-quality-en.md
      - name: why-quality-schemas
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Data & schemas
        files:
          fr: ./texts/why-gitribute/why-gitribute-quality-schemas-en.md
          en: ./texts/why-gitribute/why-gitribute-quality-schemas-en.md
      - name: why-quality-consolidation
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Data consolidation
        files:
          fr: ./texts/why-gitribute/why-gitribute-quality-consolidation-en.md
          en: ./texts/why-gitribute/why-gitribute-quality-consolidation-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: how-it-works
    url: /how-it-works
    options:
      hero: true
      summary: true
      contrib: true
      name:
        en: How it works
    sections: 
      - name: how
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/why-gitribute/how-it-works-en.md
          en: ./texts/why-gitribute/how-it-works-en.md
      - name: how-widgets-collection
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: A widgets collection
        files:
          fr: ./texts/why-gitribute/how-it-works-widgets-collection-en.md
          en: ./texts/why-gitribute/how-it-works-widgets-collection-en.md
      - name: how-git-providers
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Git providers
        files:
          fr: ./texts/why-gitribute/how-it-works-git-providers-en.md
          en: ./texts/why-gitribute/how-it-works-git-providers-en.md
      - name: how-no-account
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Contribute anonymously
        files:
          fr: ./texts/why-gitribute/how-it-works-no-account-en.md
          en: ./texts/why-gitribute/how-it-works-no-account-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: main-features
    url: /main-features
    options:
      summary: true
      contrib: true
      name:
        en: Main features
    sections: 
      - name: main-features
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/why-gitribute/main-features-en.md
          en: ./texts/why-gitribute/main-features-en.md
      - name: main-features-edit
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit & contribute online
        files:
          fr: ./texts/why-gitribute/main-features-edit-en.md
          en: ./texts/why-gitribute/main-features-edit-en.md
      - name: main-features-share
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Share your datasets
        files:
          fr: ./texts/why-gitribute/main-features-share-en.md
          en: ./texts/why-gitribute/main-features-share-en.md
      - name: main-features-adapt
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Adapt the widgets to your needs
        files:
          fr: ./texts/why-gitribute/main-features-adapt-en.md
          en: ./texts/why-gitribute/main-features-adapt-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: roadmap
    url: /roadmap
    options:
      contrib: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/roadmap-en.md
          en: ./texts/why-gitribute/roadmap-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /stack
              icon-left: xml
              rounded: true
              label: 
                fr: Stack
                en: Stack
            - link: https://gitlab.com/multi-coop/gitribute
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: architecture
    url: /architecture
    options:
      summary: true
      contrib: true
      name:
        en: Architecture & sketches
    sections: 
      - name: architecture-schemas-intro
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Sketches & wireframes
        files:
          fr: ./texts/why-gitribute/architecture-schemas-intro-en.md
          en: ./texts/why-gitribute/architecture-schemas-intro-en.md
      - name: architecture
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Main ideas
        files:
          fr: ./texts/why-gitribute/architecture-en.md
          en: ./texts/why-gitribute/architecture-en.md
      - name: architecture-git-providers
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Git providers as database
        files:
          fr: ./texts/why-gitribute/architecture-git-providers-en.md
          en: ./texts/why-gitribute/architecture-git-providers-en.md
      - name: architecture-basic-interoperability
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Basic interoperability
        files:
          fr: ./texts/why-gitribute/architecture-basic-interoperability-en.md
          en: ./texts/why-gitribute/architecture-basic-interoperability-en.md
      - name: architecture-git-data-agnostic
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Data agnostic
        files:
          fr: ./texts/why-gitribute/architecture-data-agnostic-en.md
          en: ./texts/why-gitribute/architecture-data-agnostic-en.md
      - name: architecture-widgets-collection
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: A widgets collection...
        files:
          fr: ./texts/why-gitribute/architecture-widgets-collection-en.md
          en: ./texts/why-gitribute/architecture-widgets-collection-en.md
      - name: architecture-for-noobs
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: ...For noobs
        files:
          fr: ./texts/why-gitribute/architecture-for-noobs-en.md
          en: ./texts/why-gitribute/architecture-for-noobs-en.md
      - name: architecture-schemas-wireframes
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Components wireframes
        files:
          fr: ./texts/why-gitribute/architecture-schemas-wireframes-en.md
          en: ./texts/why-gitribute/architecture-schemas-wireframes-en.md
      - name: architecture-schemas-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Widget for `csv` preview and edition
        files:
          fr: ./texts/why-gitribute/architecture-schemas-csv-en.md
          en: ./texts/why-gitribute/architecture-schemas-csv-en.md
      - name: architecture-schemas-md
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Widget for `md` preview and edition
        files:
          fr: ./texts/why-gitribute/architecture-schemas-md-en.md
          en: ./texts/why-gitribute/architecture-schemas-md-en.md
      - name: architecture-schemas-save-dialog
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Dialog before saving changes
        files:
          fr: ./texts/why-gitribute/architecture-schemas-save-dialog-en.md
          en: ./texts/why-gitribute/architecture-schemas-save-dialog-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /stack
              icon-left: xml
              rounded: true
              label: 
                fr: Stack
                en: Stack
            - link: https://gitlab.com/multi-coop/gitribute
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: stack
    url: /stack
    options:
      contrib: true
    sections: 
      - name: docs-stack
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/why-gitribute/stack-en.md
          en: ./texts/why-gitribute/stack-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /roadmap
              icon-left: map-search-outline
              rounded: true
              label: 
                fr: Roadmap
                en: Roadmap
            - link: https://gitlab.com/multi-coop/gitribute
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: business-model
    url: /business-model
    options:
      # hero: true
      summary: true
      contrib: true
      name:
        en: Business-model
    sections: 
      - name: business-model
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Business model
        files:
          fr: ./texts/why-gitribute/business-model-en.md
          en: ./texts/why-gitribute/business-model-en.md
      - name: business-model-no_trap
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: No trap, just open source
        files:
          fr: ./texts/why-gitribute/business-model-no_trap-en.md
          en: ./texts/why-gitribute/business-model-no_trap-en.md
      - name: business-model-idea
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: An idea, and the quick proof it could technically work
        files:
          fr: ./texts/why-gitribute/business-model-idea-en.md
          en: ./texts/why-gitribute/business-model-idea-en.md
      - name: business-model-usecases
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Real use cases
        files:
          fr: ./texts/why-gitribute/business-model-usecases-en.md
          en: ./texts/why-gitribute/business-model-usecases-en.md
      - name: business-model-mutualize
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Mutualize & converge with the roadmap 
        files:
          fr: ./texts/why-gitribute/business-model-mutualize-en.md
          en: ./texts/why-gitribute/business-model-mutualize-en.md
      - name: business-model-valorize
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Valorize the expertise, not the code
        files:
          fr: ./texts/why-gitribute/business-model-valorize-en.md
          en: ./texts/why-gitribute/business-model-valorize-en.md
      - name: clients
        component: TextComponent
        options:
          columns-size: full
          name:
            en: They support Gitribute
        files:
          fr: ./texts/landing/landing-clients.md
          en: ./texts/landing/landing-clients.md
      - name: contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  
  # BENCHMARK
  - name: benchmark
    url: /benchmark
    options:
      contrib: true
      summary: true
      name:
        en: Benchmark
    sections: 
      - name: benchmark-head
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Introduction
        files:
          en: ./texts/benchmark/benchmark-head-en.md
      - name: benchmark-comparisons
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Comparisons
        files:
          en: ./texts/benchmark/benchmark-comparisons-en.md
      - name: benchmark-comparisons-open
        component: TextComponent
        options:
          columns-size: full
          depth: 1
          name:
            en: Open source solutions
        files:
          en: ./texts/benchmark/benchmark-comparisons-open-en.md
      - name: benchmark-comparisons-proprietary
        component: TextComponent
        options:
          columns-size: full
          depth: 1
          name:
            en: Proprietary solutions
        files:
          en: ./texts/benchmark/benchmark-comparisons-proprietary-en.md
      - name: benchmark-solutions
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Solutions
        files:
          en: ./texts/benchmark/benchmark-solutions-en.md
      - name: benchmark-data
        component: DataGrid
        options:
          columns-size: full
          depth: 1
          name:
            en: Grid list
        files:
          en: ./texts/benchmark/benchmark-data.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # TUTORIAL
  - name: tutorial-overview
    url: /tutorial-overview
    options:
      summary: true
      contrib: true
      name:
        en: Tutorials overview
    sections: 
      - name: tutorial-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/tutorial/tutorial-overview-en.md
          en: ./texts/tutorial/tutorial-overview-en.md
      - name: tutorial-overview-actions
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Main actions
        files:
          fr: ./texts/tutorial/tutorial-overview-actions-en.md
          en: ./texts/tutorial/tutorial-overview-actions-en.md
      - name: tutorial-overview-edition
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edition
        files:
          fr: ./texts/tutorial/tutorial-overview-edition-en.md
          en: ./texts/tutorial/tutorial-overview-edition-en.md
      - name: tutorial-overview-contribution
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Contribution
        files:
          fr: ./texts/tutorial/tutorial-overview-contribution-en.md
          en: ./texts/tutorial/tutorial-overview-contribution-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: tutorial-actions
    url: /tutorial-actions
    options:
      summary: true
      contrib: true
      name:
        en: Actions features
    sections: 
      - name: tutorial-actions
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/tutorial/tutorial-actions-en.md
          en: ./texts/tutorial/tutorial-actions-en.md
      - name: tutorial-actions-file-infos
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: File's informations
        files:
          fr: ./texts/tutorial/tutorial-actions-file-infos-en.md
          en: ./texts/tutorial/tutorial-actions-file-infos-en.md
      - name: tutorial-actions-user-options
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: User's options
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-en.md
      - name: tutorial-actions-user-options-reload
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Reload the source file
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-reload-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-reload-en.md
      - name: tutorial-actions-user-options-download
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Download the file
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-download-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-download-en.md
      - name: tutorial-actions-user-options-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Change your user token
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-usertoken-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-usertoken-en.md
      - name: tutorial-actions-user-options-branches
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Check your branches
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-branches-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-branches-en.md
      - name: tutorial-actions-user-options-copy
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Copy the widget
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-copy-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-copy-en.md
      - name: tutorial-actions-user-options-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Change the language
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-locale-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-locale-en.md
      - name: tutorial-actions-change-modes
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The view modes
        files:
          fr: ./texts/tutorial/tutorial-actions-change-modes-en.md
          en: ./texts/tutorial/tutorial-actions-change-modes-en.md
      - name: tutorial-actions-edit-modes
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Switch the "edit-view" modes
        files:
          fr: ./texts/tutorial/tutorial-actions-edit-modes-en.md
          en: ./texts/tutorial/tutorial-actions-edit-modes-en.md
      - name: tutorial-actions-edit-modes-preview
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "Preview" mode
        files:
          fr: ./texts/tutorial/tutorial-actions-edit-modes-preview-en.md
          en: ./texts/tutorial/tutorial-actions-edit-modes-preview-en.md
      - name: tutorial-actions-edit-modes-edit
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "Edit" mode
        files:
          fr: ./texts/tutorial/tutorial-actions-edit-modes-edit-en.md
          en: ./texts/tutorial/tutorial-actions-edit-modes-edit-en.md
      - name: tutorial-actions-edit-modes-diff
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "Diff" mode
        files:
          fr: ./texts/tutorial/tutorial-actions-edit-modes-diff-en.md
          en: ./texts/tutorial/tutorial-actions-edit-modes-diff-en.md
      - name: tutorial-actions-cards_view
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Cards view
        files:
          fr: ./texts/tutorial/tutorial-actions-cards_view-en.md
          en: ./texts/tutorial/tutorial-actions-cards_view-en.md
      - name: tutorial-actions-search_filters
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Search and filter
        files:
          fr: ./texts/tutorial/tutorial-actions-search_filters-en.md
          en: ./texts/tutorial/tutorial-actions-search_filters-en.md
      - name: tutorial-actions-search
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Fulltext search
        files:
          fr: ./texts/tutorial/tutorial-actions-search-en.md
          en: ./texts/tutorial/tutorial-actions-search-en.md
      - name: tutorial-actions-filters
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Filters
        files:
          fr: ./texts/tutorial/tutorial-actions-filters-en.md
          en: ./texts/tutorial/tutorial-actions-filters-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: tutorial-edition
    url: /tutorial-edition
    options:
      summary: true
      contrib: true
      name:
        en: Edition features
    sections: 
      - name: edition
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/tutorial/tutorial-edition-en.md
          en: ./texts/tutorial/tutorial-edition-en.md
      - name: edition-md
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a markdown file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-md-en.md
          en: ./texts/tutorial/tutorial-edition-edit-md-en.md
      - name: edition-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a CSV file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-csv-en.md
          en: ./texts/tutorial/tutorial-edition-edit-csv-en.md
      - name: edition-csv-fields
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Table fields
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-csv-fields-en.md
          en: ./texts/tutorial/tutorial-edition-edit-csv-fields-en.md
      - name: edition-csv-rows
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Common rows operations
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-csv-rows-en.md
          en: ./texts/tutorial/tutorial-edition-edit-csv-rows-en.md
      - name: edition-csv-consolidation_field
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Consolidation field
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-csv-consolidation_field-en.md
          en: ./texts/tutorial/tutorial-edition-edit-csv-consolidation_field-en.md
      - name: edition-json
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a JSON file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-json-en.md
          en: ./texts/tutorial/tutorial-edition-edit-json-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: tutorial-contribution
    url: /tutorial-contribution
    options:
      summary: true
      contrib: true
      name:
        en: Contribution features
    sections: 
      - name: contribution
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/tutorial/tutorial-contribution-en.md
          en: ./texts/tutorial/tutorial-contribution-en.md
      - name: contribution-what
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: What is a contribution ?
        files:
          fr: ./texts/tutorial/tutorial-contribution-what-en.md
          en: ./texts/tutorial/tutorial-contribution-what-en.md
      - name: contribution-send
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Send your contribution
        files:
          fr: ./texts/tutorial/tutorial-contribution-send-en.md
          en: ./texts/tutorial/tutorial-contribution-send-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # DOCUMENTATION
  - name: install
    url: /install
    options:
      summary: true
      contrib: true
      name:
        en: Installation strategies
    sections: 
      - name: installation
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
           en: Introduction
        files:
          fr: ./texts/installation/installation-en.md
          en: ./texts/installation/installation-en.md
      - name: installation-reuse
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
           en: Reuse some widgets
        files:
          fr: ./texts/installation/installation-reuse-en.md
          en: ./texts/installation/installation-reuse-en.md
      - name: installation-adapt
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
           en: Adapt Gitribute for your website
        files:
          fr: ./texts/installation/installation-adapt-en.md
          en: ./texts/installation/installation-adapt-en.md
      - name: installation-instance
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
           en: Install your instance
        files:
          fr: ./texts/installation/installation-instance-en.md
          en: ./texts/installation/installation-instance-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: https://gitlab.com/multi-coop/gitribute
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: quickstart-developpers
    url: /quickstart-developpers
    options:
      contrib: true
    sections: 
      - name: setup
        component: TextComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/installation/setup-en.md
          en: ./texts/installation/setup-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: https://gitlab.com/multi-coop/gitribute
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: integration
    url: /integration
    options:
      hero: true
      contrib: true
    sections: 
      - name: integration
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/installation/integration-en.md
          en: ./texts/installation/integration-en.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # WIDGETS
  - name: docs-widgets-overview
    url: /docs-widgets-overview
    options:
      summary: true
      contrib: true
      name:
        en: Widgets overview
    sections: 
      - name: docs-widgets-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introduction
        files:
          fr: ./texts/documentation/docs-widgets-overview-en.md
          en: ./texts/documentation/docs-widgets-overview-en.md
      - name: docs-widgets-overview-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "gitfile" widget
        files:
          fr: ./texts/documentation/docs-gitfile-en.md
          en: ./texts/documentation/docs-gitfile-en.md
      - name: btn-gitfile
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          not-in-menu: true
          custom-class: mb-6
          buttons:
            - link: /docs-gitfile
              icon-left: book-open-variant
              rounded: true
              label: 
                fr: Gitfile widget
                en: Gitfile widget
      - name: docs-widgets-overview-multifiles
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "multi-files" widget
        files:
          fr: ./texts/documentation/docs-multi-files-en.md
          en: ./texts/documentation/docs-multi-files-en.md
      - name: btn-multi-files
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          not-in-menu: true
          custom-class: mb-6
          buttons:
            - link: /docs-multi-files
              icon-left: book-open-variant
              rounded: true
              label: 
                fr: Multi-files widget
                en: Multi-files widget
      - name: docs-widgets-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "explowiki" widget
        files:
          fr: ./texts/documentation/docs-explowiki-en.md
          en: ./texts/documentation/docs-explowiki-en.md
      - name: btn-explowiki
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          not-in-menu: true
          custom-class: mb-6
          buttons:
            - link: /docs-explowiki
              icon-left: book-open-variant
              rounded: true
              label: 
                fr: Explowiki widget
                en: Explowiki widget
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: docs-gitfile
    url: /docs-gitfile
    options:
      summary: true
      contrib: true
      name:
        en: The "gitfile" widget
    sections: 
      - name: docs-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Presentation
        files:
          fr: ./texts/documentation/docs-gitfile-en.md
          en: ./texts/documentation/docs-gitfile-en.md
      - name: docs-gitfile-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Structure
        files:
          fr: ./texts/documentation/docs-gitfile-structure-en.md
          en: ./texts/documentation/docs-gitfile-structure-en.md
      - name: docs-gitfile-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Example
        files:
          fr: ./texts/documentation/docs-gitfile-structure-example-en.md
          en: ./texts/documentation/docs-gitfile-structure-example-en.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Parameters
        files:
          fr: ./texts/documentation/docs-params/params-en.md
          en: ./texts/documentation/docs-params/params-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "height" parameter
        files:
          fr: ./texts/documentation/docs-params/param-height.md
          en: ./texts/documentation/docs-params/param-height.md
      - name: docs-param-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "gitfile" parameter
        files:
          fr: ./texts/documentation/docs-params/param-gitfile.md
          en: ./texts/documentation/docs-params/param-gitfile.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "usertoken" parameter
        files:
          fr: ./texts/documentation/docs-params/param-usertoken.md
          en: ./texts/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-git
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Notes about the "usertoken" parameter
        files:
          fr: ./texts/documentation/docs-params/param-usertoken-notes-git.md
          en: ./texts/documentation/docs-params/param-usertoken-notes-git.md
      - name: docs-param-onlypreview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "onlypreview" parameter
        files:
          fr: ./texts/documentation/docs-params/param-onlypreview.md
          en: ./texts/documentation/docs-params/param-onlypreview.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "locale" parameter
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "debug" parameter
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "options" parameter
        files:
          fr: ./texts/documentation/docs-options/option-global.md
          en: ./texts/documentation/docs-options/option-global.md
      - name: docs-option-gitfile-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "options" keys for table files
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-csv.md
          en: ./texts/documentation/docs-options/option-gitfile-csv.md
      - name: docs-option-gitfile-custom_props
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Custom properties file for table files
        files:
          fr: ./texts/documentation/docs-custom-props/props-custom_props.md
          en: ./texts/documentation/docs-custom-props/props-custom_props.md
      - name: docs-option-gitfile-json
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "options" keys for json files
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-json.md
          en: ./texts/documentation/docs-options/option-gitfile-json.md
      - name: docs-option-gitfile-md
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "options" keys for md files
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-md.md
          en: ./texts/documentation/docs-options/option-gitfile-md.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: docs-explowiki
    url: /docs-explowiki
    options:
      summary: true
      contrib: true
      name:
        en: The "explowiki" widget
    sections: 
      - name: docs-explowiki
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Presentation
        files:
          fr: ./texts/documentation/docs-explowiki-en.md
          en: ./texts/documentation/docs-explowiki-en.md
      - name: docs-explowiki-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Structure
        files:
          fr: ./texts/documentation/docs-explowiki-structure-en.md
          en: ./texts/documentation/docs-explowiki-structure-en.md
      - name: docs-explowiki-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Example
        files:
          fr: ./texts/documentation/docs-explowiki-structure-example-en.md
          en: ./texts/documentation/docs-explowiki-structure-example-en.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Parameters
        files:
          fr: ./texts/documentation/docs-params/params-en.md
          en: ./texts/documentation/docs-params/params-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "height" parameter
        files:
          fr: ./texts/documentation/docs-params/param-height.md
          en: ./texts/documentation/docs-params/param-height.md
      - name: docs-param-wikilist
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "wikilist" parameter
        files:
          fr: ./texts/documentation/docs-params/param-wikilist.md
          en: ./texts/documentation/docs-params/param-wikilist.md
      - name: docs-param-wikipages
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "wikipages" parameter
        files:
          fr: ./texts/documentation/docs-params/param-wikipages.md
          en: ./texts/documentation/docs-params/param-wikipages.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "usertoken" parameter
        files:
          fr: ./texts/documentation/docs-params/param-usertoken.md
          en: ./texts/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-mediawiki
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Notes about the "usertoken" parameter
        files:
          fr: ./texts/documentation/docs-params/param-usertoken-notes-mediawiki.md
          en: ./texts/documentation/docs-params/param-usertoken-notes-mediawiki.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "locale" parameter
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "debug" parameter
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "options" parameter
        files:
          fr: ./texts/documentation/docs-options/option-global.md
          en: ./texts/documentation/docs-options/option-global.md
      - name: docs-option-explowiki-table
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "options" keys for wiki data
        files:
          fr: ./texts/documentation/docs-options/option-explowiki-table.md
          en: ./texts/documentation/docs-options/option-explowiki-table.md
      - name: docs-option-explowiki-custom_props
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Custom properties file for wiki data
        files:
          fr: ./texts/documentation/docs-custom-props/props-custom_props.md
          en: ./texts/documentation/docs-custom-props/props-custom_props.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: docs-multi-files
    url: /docs-multi-files
    options:
      summary: true
      contrib: true
      name:
        en: The "multi-files" widget
    sections: 
      - name: docs-multi-files
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Presentation
        files:
          fr: ./texts/documentation/docs-multi-files-en.md
          en: ./texts/documentation/docs-multi-files-en.md
      - name: docs-multi-files-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Structure
        files:
          fr: ./texts/documentation/docs-multi-files-structure-en.md
          en: ./texts/documentation/docs-multi-files-structure-en.md
      - name: docs-multi-files-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: Example
        files:
          fr: ./texts/documentation/docs-multi-files-structure-example-en.md
          en: ./texts/documentation/docs-multi-files-structure-example-en.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Parameters
        files:
          fr: ./texts/documentation/docs-params/params-en.md
          en: ./texts/documentation/docs-params/params-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "height" parameter
        files:
          fr: ./texts/documentation/docs-params/param-height.md
          en: ./texts/documentation/docs-params/param-height.md
      - name: docs-param-gitfiles
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "gitfiles" parameter
        files:
          fr: ./texts/documentation/docs-params/param-gitfiles.md
          en: ./texts/documentation/docs-params/param-gitfiles.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "locale" parameter
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "debug" parameter
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "options" parameter
        files:
          fr: ./texts/documentation/docs-options/option-global.md
          en: ./texts/documentation/docs-options/option-global.md
      - name: docs-option-multifiles
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            en: The "options" keys for multi-files
        files:
          fr: ./texts/documentation/docs-options/option-multifiles.md
          en: ./texts/documentation/docs-options/option-multifiles.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # STANDARD ROUTES
  - name: contact
    url: /contact
    options:
      hero: true
    sections: 
      - name: contact
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/contact/contact-head-fr.md
          en: ./texts/contact/contact-head-en.md

  - name: contribute
    url: /contribute
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
          columns-divider: h1
        files:
          fr: ./texts/contact/contribute-head-fr.md
          en: ./texts/contact/contribute-head-fr.md

  - name: legal
    url: /legal
    sections: 
      # - name: data
      #   component: TextDataComponent
      #   files:
      #     fr: ./texts/contact/legal-data.md
      - name: legal-text
        component: TextComponent
        files:
          fr: ./texts/contact/legal-mentions-fr.md
          en: ./texts/contact/legal-mentions-fr.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # GALLERY
  - name: gitribute-odf-observatoire
    url: /gitribute-odf-observatoire
    sections: 
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: full
          js: 
            - href: https://gitribute.multi.coop/js/app.js
          css: 
            - href: https://gitribute.multi.coop/css/app.css
          html: |
            <multi-gitribute-multi-files 
              title="test multi-files observatoire" 
              debug="false"
              locale="fr" 
              options='{
                "display": "horizontal"
              }' gitfiles='[
              {
                "title": "Données de l&#39;observatoire",
                "activate": true,
                "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-Observatoire-apiviz_data-export_solidata-220425b-simplified.csv",
                "default-tab": true,
                "options": {
                  "height": "500px",
                  "separator": ";",
                  "lockcolumns": true,
                  "customfilters": {
                    "activate": true, 
                    "filterfields" : [ 
                      "type",
                      "platform_clean",
                      "depcode"
                    ]
                  },
                  "schema": {
                    "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-Observatoire-apiviz_data-schema.json"
                  },
                  "fields-custom-properties": {
                    "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-Observatoire-apiviz_data-fields-custom-props.json"
                  },
                  "cardsview": { 
                    "activate": true,
                    "default" : false
                  },
                  "cardsdetail": true,
                  "cardssettings": {
                    "mini": {
                      "nom": { "position": "title" },
                      "siren" : { "position": "resume" },
                      "tags" : { "position": "tags" } 
                    },
                    "detail": {
                      "nom": { "position": "title" },
                      "orga": { "position": "resume" },
                      "siren": { "position": "description" },
                      "adress": { "position": "description" },
                      "dep_label": { "position": "tags" },
                      "tags" : { "position": "tags" }
                    }
                  }
                },
                "usertoken": ""
              },
              {
                "title": "Thématiques",
                "activate": true,
                "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-Observatoire-thematiques.csv",
                "options": {
                  "height": "500px",
                  "separator": ",",
                  "lockcolumns": true,
                  "customfilters": {
                    "activate": true, 
                    "filterfields" : [ 
                      "Tags",
                      "Organisations_Noms"
                    ]
                  },
                  "schema": {
                    "fields": [
                      {
                        "name": "Organisations copy",
                        "type": "boolean"
                      }
                    ]
                  },
                  "fields-custom-properties": {
                    "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-thematiques-fields-custom-props.json"
                  }
                },
                "onlypreview": true,
                "usertoken": ""
              },
              {
                "title": "Schéma des données de l&#39;observatoire",
                "activate": true,
                "default-tab": false,
                "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-Observatoire-apiviz_data-schema.json",
                "options": {
                  "defaultDepth": 2,
                  "allowKeyEdit": true
                },  
                "onlypreview": false,
                "usertoken": ""
              },
              {
                "title": "Présentation de l&#39;Observatoire de l&#39;Open data",
                "activate": true,
                "gitfile": "https://github.com/multi-coop/gitribute-content-test/blob/main/texts/markdown/odf/ODF-observatoire-intro.md",
                "options": ""
              }
            ]'></multi-gitribute-multi-files>
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: gitribute-odf-ressources
    url: /gitribute-odf-ressources
    sections: 
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: full
          js: 
            - href: https://gitribute.multi.coop/js/app.js
          css: 
            - href: https://gitribute.multi.coop/css/app.css
          html: |
            <multi-gitribute-file
              gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/odf/ODF-liste des ressources.csv"
              options='{
                "height": "500px",
                "separator": ",",
                "lockcolumns": true,
                "tagseparator": ",",
                "customfilters": {
                  "activate": true,
                  "filterfields": [
                    "Type",
                    "Enjeux politiques",
                    "Enjeux Opérationnels",
                    "Phase"
                  ]
                },
                "schema": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-ressources-schema.json"
                },
                "fields-custom-properties": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/odf/ODF-ressources-fields-custom-props.json"
                },
                "customsorting" : {
                  "activate": true,
                  "sortfields": [
                    "Objet",
                    "Nom de la ressource"
                  ]
                },
                "pagination":{
                  "itemsPerPage": 20
                },
                "cardsview": {
                  "activate": true,
                  "default": false
                },
                "cardsdetail": true,
                "cardssettings": {
                  "mini": {
                    "Nom de la ressource": {"position": "title"},
                    "Objet": {"position": "resume"},
                    "Enjeux politiques": {"position": "tags"},
                    "Phases": {"position": "tags"}
                  },
                  "detail": {
                    "Nom de la ressource": {"position": "title"},
                    "Objet": {"position": "resume"},
                    "Enjeux politiques": {"position": "tags"},
                    "Phases": {"position": "tags"},
                    "Lien vers la ressources": {"position": "links"}
                  }
                }
              }' 
              title="ODF - Ressources (export airtable)"
              usertoken=""
              locale="fr"
              debug="false">
            </multi-gitribute-file>
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: gitribute-cooptech
    url: /gitribute-cooptech
    sections: 
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: full
          js: 
            - href: https://gitribute.multi.coop/js/app.js
          css: 
            - href: https://gitribute.multi.coop/css/app.css
          html: |
            <multi-gitribute-file
              title="Liste des coopératives de la tech en France - csv ( semicolon separator)"
              gitfile="https://github.com/multi-coop/gitribute-content-test/blob/main/data/csv/cooptech/Annuaire-SCOP-SCIC-tech-France.csv"
              options='{
                "height": "500px",
                "separator":",",
                "lockcolumns": true,
                "tagseparator":",",
                "customfilters" : {
                  "activate": true,
                  "filterfields": [
                  "type",
                    "Statut juridique"
                    ]
                },
                "schema": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-schema.json"
                },
                "fields-custom-properties": {
                  "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/cooptech/Annuaire-SCOP-SCIC-tech-France-fields-custom-props.json"
                },
                "customsorting" : {
                  "activate": true,
                  "sortfields": [
                    { "name": "Nom" }
                  ]
                },
                "pagination":{
                  "itemsPerPage": 20
                },
                "cardsview": {
                  "activate": true,
                  "default": false
                },
                "cardsdetail": true,
                "cardssettings": {
                  "mini": {
                    "Nom": {"position": "title"},
                    "Présentation": {"position": "description"},
                    "Site internet": {"position": "description"},
                    "Statut juridique": {"position": "tags"},
                    "Domaine(s)": {"position": "tags"}
                  },
                  "detail": {
                    "Nom": {"position": "title"},
                    "Site internet": {"position": "description"},
                    "Présentation": {"position": "description"},
                    "Numéro SIREN": {"position": "description"},
                    "Adresse": {"position": "description"},
                    "Statut juridique": {"position": "tags"},
                    "Domaine(s)": {"position": "tags"},
                    "Fiche URSCOP": {"position": "links"}
                  }
                }
              }'
              usertoken=""
              locale="fr"
              debug="false"
            />
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: gitribute-explowiki-fabmob
    url: /gitribute-explowiki-fabmob
    sections: 
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: full
          js: 
            - href: https://gitribute.multi.coop/js/app.js
          css: 
            - href: https://gitribute.multi.coop/css/app.css
          html: |
            <multi-gitribute-explowiki
              wikilist="https://wiki.lafabriquedesmobilites.fr/wiki/Sp%C3%A9cial:WfExplore?title=Sp%C3%A9cial%3AWfExplore&page=1&wf-expl-Category-Projet=on&wf-expl-Page_creator-fulltext=&wf-expl-Tags="
              wikipages='[
                  "https://wiki.lafabriquedesmobilites.fr/wiki/Accra_Mobile",
                  "https://wiki.lafabriquedesmobilites.fr/wiki/Agremob_Self_Data_Territorial_La_Rochelle",
                  "https://wiki.lafabriquedesmobilites.fr/wiki/Autonomous_Kart_for_Student"
                ]' options='{
                  "height": "700px",
                  "schema": {
                    "file": "https://github.com/multi-coop/gitribute-content-test/blob/main/data/json/fabmob/fabmob-projets-schema.json"
                  },
                  "fields-custom-properties": {
                    "fields": [
                      { 
                        "name": "pageUrl",
                        "subtype": "link",
                        "locked": true
                      },
                      { 
                        "name": "imageUrl",
                        "subtype": "link"
                      },
                      { 
                        "name": "url",
                        "subtype": "link"
                      },
                      {
                        "name": "Tags",
                        "subtype": "tags",
                        "tagSeparator": ","
                      },
                      {
                        "name": "Theme",
                        "subtype": "tags",
                        "tagSeparator": ","
                      },
                      {
                        "name": "location",
                        "subtype": "tags",
                        "tagSeparator": ","
                      },
                      {
                        "name": "from",
                        "subtype": "tags",
                        "tagSeparator": ","
                      },
                      {
                        "name": "challenge",
                        "subtype": "tags",
                        "tagSeparator": ","
                      }
                    ]
                  },
                  "wikisettings": {
                    "category": "projet",
                    "fields": [
                      "url",
                      "description",
                      "shortDescription",
                      "Main_Picture",
                      "Coordonnées géo",
                      "needs",
                      "referent",
                      "communauté d&#39;intérêt",
                      "Titre",
                      "Tags",
                      "etape",
                      "Theme",
                      "location",
                      "from",
                      "challenge"
                    ],
                    "tagfields": [
                      "Tags",
                      "Theme",
                      "location",
                      "from",
                      "challenge"
                    ]
                },
                "customsorting" : {
                  "activate": true,
                  "sortfields": [
                    "title"
                  ]
                },
                "customfilters" : {
                  "activate": true,
                  "filterfields": [
                    "Tags",
                    "Theme"
                  ]
                },
                "pagination": {
                  "itemsPerPage":12
                },
                "cardsview": {
                  "activate": true,
                  "default": true
                },
                "cardssettings": {
                  "mini": {
                    "title": {"position": "title"},
                    "imageUrl": {"position": "image"},
                    "shortDescription": {"position": "resume"},
                    "Tags": {"position": "tags"},
                    "Theme": {"position": "tags"},
                    "challenge": {"position": "tags"}
                  },
                  "detail": {
                    "title": {"position": "title"},
                    "imageUrl": {"position": "image"},
                    "shortDescription": {"position": "resume"},
                    "description": {"position": "description"},
                    "Tags": {"position": "tags"},
                    "Theme": {"position": "tags"},
                    "challenge": {"position": "tags"},
                    "communauté d&#39;intérêt": {"position": "tags"},
                    "url": {"position": "links"}
                  }
                }
              }' title="gitribute for explowiki - fabmob :)" locale="fr"></multi-gitribute-explowiki>
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
--- 
