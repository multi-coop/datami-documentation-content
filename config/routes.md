---
routes: 

  # LANDING
  - name: home
    url: /
    options:
      hero: true
    sections:
      - name: logo
        component: TextComponent
        options:
          columns-size: half
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
      - name: btn-to-documentation
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons:
            - link: /tutorial-overview
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Tutorials
                en: Tutorials
            - link: /docs-gitfile
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Documentation
                en: Documentation
            - link: /source-code
              icon-left: gitlab
              rounded: true
              label: 
                fr: Code source
                en: Source code
      - name: intro
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/landing/landing-intro-en.md
          en: ./texts/landing/landing-intro-en.md
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
                "cardsview": { "activate": true, "default": false },
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
      - name: outro
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/landing/landing-outro-en.md
          en: ./texts/landing/landing-outro-en.md

  # WHAT IS GITRIBUTE
  - name: why-gitribute
    url: /why-gitribute
    options:
      hero: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/why-gitribute-en.md
          en: ./texts/why-gitribute/why-gitribute-en.md
  - name: how-it-works
    url: /how-it-works
    options:
      hero: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/how-it-works-en.md
          en: ./texts/why-gitribute/how-it-works-en.md
  - name: main-features
    url: /main-features
    options:
      summary: true
    sections: 
      - name: main-features
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Introduction
        files:
          fr: ./texts/why-gitribute/main-features-en.md
          en: ./texts/why-gitribute/main-features-en.md
      - name: main-features-edit
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Contribute to datasets
        files:
          fr: ./texts/why-gitribute/main-features-edit-en.md
          en: ./texts/why-gitribute/main-features-edit-en.md
      - name: main-features-share
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Share your datasets
        files:
          fr: ./texts/why-gitribute/main-features-share-en.md
          en: ./texts/why-gitribute/main-features-share-en.md
      - name: main-features-adapt
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Adapt the widgets to your needs
        files:
          fr: ./texts/why-gitribute/main-features-adapt-en.md
          en: ./texts/why-gitribute/main-features-adapt-en.md
  - name: roadmap
    url: /roadmap
    options: [ menu ]
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/roadmap-en.md
          en: ./texts/why-gitribute/roadmap-en.md
  - name: architecture
    url: /architecture
    options: [ menu ]
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/architecture-en.md
          en: ./texts/why-gitribute/architecture-en.md
  - name: stack
    url: /stack
    sections: 
      - name: docs-stack
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/why-gitribute/stack-en.md
          en: ./texts/why-gitribute/stack-en.md

  # - name: team 
  #   url: /team
  #   sections: 
  #     - name: head
  #       component: TextComponent
  #       options:
  #         columns-size: two-thirds
  #       files:
  #         fr: ./texts/team/team-head-fr.md
  #         en: ./texts/team/team-head-fr.md
  #     - name: data
  #       component: DataGrid
  #       files:
  #         fr: ./texts/team/team-data.md
  #         en: ./texts/team/team-data.md

  # TUTORIAL
  - name: tutorial-overview
    url: /tutorial-overview
    options:
      hero: true
    sections: 
      - name: tutorial-overview
        component: TextComponent
        options:
          columns-size: three-fourths
        files:
          fr: ./texts/tutorial/tutorial-overview-en.md
          en: ./texts/tutorial/tutorial-overview-en.md
  - name: tutorial-actions
    url: /tutorial-actions
    options:
      summary: true
    sections: 
      - name: tutorial-actions
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Introduction
        files:
          fr: ./texts/tutorial/tutorial-actions-en.md
          en: ./texts/tutorial/tutorial-actions-en.md
      - name: tutorial-actions-file-infos
        component: TextComponent
        options:
          columns-size: full
          name:
            en: File's informations
        files:
          fr: ./texts/tutorial/tutorial-actions-file-infos-en.md
          en: ./texts/tutorial/tutorial-actions-file-infos-en.md
      - name: tutorial-actions-copy-widget
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Copy the widget html block
        files:
          fr: ./texts/tutorial/tutorial-actions-copy-widget-en.md
          en: ./texts/tutorial/tutorial-actions-copy-widget-en.md
      - name: tutorial-actions-user-options
        component: TextComponent
        options:
          columns-size: full
          name:
            en: User's options
        files:
          fr: ./texts/tutorial/tutorial-actions-user-options-en.md
          en: ./texts/tutorial/tutorial-actions-user-options-en.md
      - name: tutorial-actions-edit-modes
        component: TextComponent
        options:
          columns-size: full
          name:
            en: Change view and edit modes
        files:
          fr: ./texts/tutorial/tutorial-actions-edit-modes-en.md
          en: ./texts/tutorial/tutorial-actions-edit-modes-en.md
  - name: tutorial-edition
    url: /tutorial-edition
    options:
      summary: true
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
      - name: edition-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a CSV file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-csv-en.md
          en: ./texts/tutorial/tutorial-edition-edit-csv-en.md
      - name: edition-json
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a JSON file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-json-en.md
          en: ./texts/tutorial/tutorial-edition-edit-json-en.md
      - name: edition-md
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Edit a markdown file
        files:
          fr: ./texts/tutorial/tutorial-edition-edit-md-en.md
          en: ./texts/tutorial/tutorial-edition-edit-md-en.md
  - name: tutorial-contribution
    url: /tutorial-contribution
    options:
      summary: true
    sections: 
      - name: contribution
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: Introdution
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

  # DOCUMENTATION
  - name: install
    url: /install
    options:
      summary: true
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
  - name: quickstart-developpers
    url: /quickstart-developpers
    sections: 
      - name: setup
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/installation/setup-en.md
          en: ./texts/installation/setup-en.md
  - name: integration
    url: /integration
    options:
      hero: true
    sections: 
      - name: integration
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/installation/integration-en.md
          en: ./texts/installation/integration-en.md

  # WIDGETS
  - name: docs-widgets-overview
    url: /docs-widgets-overview
    options:
      summary: true
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
            en: The "file" widget
        files:
          fr: ./texts/documentation/docs-widgets-overview-gitfile-en.md
          en: ./texts/documentation/docs-widgets-overview-gitfile-en.md
      - name: docs-widgets-overview-multifiles
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "multi-files" widget
        files:
          fr: ./texts/documentation/docs-widgets-overview-multifiles-en.md
          en: ./texts/documentation/docs-widgets-overview-multifiles-en.md
      - name: docs-widgets-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "explowiki" widget
        files:
          fr: ./texts/documentation/docs-widgets-overview-explowiki-en.md
          en: ./texts/documentation/docs-widgets-overview-explowiki-en.md
  - name: docs-gitfile
    url: /docs-gitfile
    options:
      summary: true
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
  - name: docs-explowiki
    url: /docs-explowiki
    options:
      summary: true
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
  - name: docs-multi-files
    url: /docs-multi-files
    options:
      summary: true
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

  - name: products
    url: /products
    sections: 
      - name: products-head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/references/products-head-fr.md
          en: ./texts/references/products-head-fr.md
      - name: products-data
        component: DataGrid
        files:
          fr: ./texts/references/products-data.md
          en: ./texts/references/products-data.md
      - name: btn-to-offer
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: full
          buttons: 
            - link: /offer
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Notre offre de service
                en: Our services

  - name: references
    url: /references
    sections: 
      - name: btn-to-offer-products
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-classes: mb-6
          buttons: 
            - link: /offer
              icon-left: arrow-right-bold
              rounded: true
              outlined: false
              color: light
              label: 
                fr: Notre offre de service
                en: Our services
            - link: /products
              icon-left: arrow-right-bold
              rounded: true
              outlined: false
              color: light
              label: 
                fr: Nos produits open source
                en: Our open source products
      - name: refs-head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/references/references-head-fr.md
          en: ./texts/references/references-head-fr.md
      - name: refs-data
        component: DataGrid
        files:
          fr: ./texts/references/references-data.md
          en: ./texts/references/references-data.md

  - name: contact
    url: /contact
    options:
      hero: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: full
          columns-divider: h1
        files:
          fr: ./texts/contact/contact-head-fr.md
          en: ./texts/contact/contact-head-en.md
      # - name: btn-to-jobs
      #   component: ButtonsComponent
      #   options:
      #     columns-size: full
      #     buttons-size: full
      #     buttons: 
      #       - link: /contribute
      #         icon-left: arrow-right-bold
      #         rounded: true
      #         label: 
      #           fr: Contribuer
      #           en: Contribute

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

  # JOBS
  - name: join 
    url: /join
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/jobs/join-head-fr.md
          en: ./texts/jobs/join-head-fr.md
      - name: btn-to-jobs
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: full
          buttons: 
            - link: /team
              icon-left: arrow-right-bold
              rounded: true
              outlined: true
              label: 
                fr: Découvrez l'équipe
                en: Discover the team
            - link: /jobs
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Nos offres d'emploi
                en: Our job offers

  - name: jobs 
    url: /jobs
    sections: 
      - name: btn-to-join
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: two-thirds
          custom-classes: mb-5
          buttons: 
            - link: /join
              icon-left: arrow-right-bold
              rounded: true
              outlined: true
              label: 
                fr: Pourquoi rejoindre multi ?
                en: Why joining multi ?
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/jobs/jobs-head-fr.md
          en: ./texts/jobs/jobs-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/jobs/jobs-data.md
          en: ./texts/jobs/jobs-data.md


  - name: blog
    url: /blog
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/blog/blog-head-fr.md
          en: ./texts/blog/blog-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/blog/blog-data.md
          en: ./texts/blog/blog-data.md

  - name: network
    url: /network
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/network/network-head-fr.md
          en: ./texts/network/network-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/network/network-data.md
          en: ./texts/network/network-data.md

  - name: ressources
    url: /ressources
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/ressources/ressources-head-fr.md
          en: ./texts/ressources/ressources-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/ressources/ressources-data.md
          en: ./texts/ressources/ressources-data.md

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
                "cardsview": { "activate": true, "default": false },
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
                "cardsview": { "activate": true, "default": false },
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
--- 
