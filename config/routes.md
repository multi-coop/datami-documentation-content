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
          columns-size: full
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

  # WHAT IS GITRIBUTE
  - name: why
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
    sections: 
      - name: tutorial-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
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
            en: Change edit mode
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
  - name: quickstart
    url: /quickstart
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
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
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
          name:
            en: Notes about the "usertoken" parameter
        files:
          fr: ./texts/documentation/docs-params/param-usertoken-notes-git.md
          en: ./texts/documentation/docs-params/param-usertoken-notes-git.md
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
          name:
            en: The "options" for csv files
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-csv.md
          en: ./texts/documentation/docs-options/option-gitfile-csv.md
      - name: docs-option-gitfile-json
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "options" for json files
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-json.md
          en: ./texts/documentation/docs-options/option-gitfile-json.md
      - name: docs-option-gitfile-md
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "options" for md files
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
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
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
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            en: The "title" parameter
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
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

  - name: shares-simulator
    url: /shares-simulator
    sections: 
      - name: simulator
        component: WidgetComponent
        options:
          columns-size: two-thirds
          js: 
            - href: https://multi-site-simulator-test.netlify.app/js/app.js
          css: 
            - href: https://multi-site-simulator-test.netlify.app/css/app.css
          html: |
            <multi-shares-simulator 
              locale="fr"
              cooperative="multi"
              partvalue="25"
              minbenefs="0"
              benefs="100000"
              repart='{
                "reserves":40,
                "participation":50,
                "dividendes":10
              }'
              team='[
                { "name":"Johan Richer", "parts":100, "workTime":100, "yearTime": 12 },
                { "name":"Julien Paris", "parts":100, "workTime":100, "yearTime": 12 },
                { "name":"Thomas Brosset", "parts":40, "workTime":40, "yearTime": 12 },
                { "name":"Pierre Camilleri", "parts":100, "workTime":60, "yearTime": 12 },
                { "name":"Quentin Loridant", "parts": 100, "workTime":80, "yearTime": 12 }
              ]'
            />
--- 
