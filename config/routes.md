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
    options: [ menu ]
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
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/main-features-en.md
          en: ./texts/why-gitribute/main-features-en.md
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
    sections: 
      - name: actions
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/tutorial/tutorial-actions-en.md
          en: ./texts/tutorial/tutorial-actions-en.md
  - name: tutorial-edition
    url: /tutorial-edition
    sections: 
      - name: edition
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/tutorial/tutorial-edition-en.md
          en: ./texts/tutorial/tutorial-edition-en.md
  - name: tutorial-contribution
    url: /tutorial-contribution
    sections: 
      - name: contribution
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/tutorial/tutorial-contribution-en.md
          en: ./texts/tutorial/tutorial-contribution-en.md

  # DOCUMENTATION
  - name: docs-installation
    url: /docs-installation
    sections: 
      - name: installation
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-installation-en.md
          en: ./texts/documentation/docs-installation-en.md
      # - name: btn-to-products
      #   component: ButtonsComponent
      #   options:
      #     columns-size: two-thirds
      #     buttons-size: half
      #     buttons: 
      #       - link: /products
      #         icon-left: arrow-right-bold
      #         rounded: true
      #         label: 
      #           fr: Nos produits open source
      #           en: Our open source products
      #       - link: /references
      #         icon-left: arrow-right-bold
      #         rounded: true
      #         label: 
      #           fr: Nos références
      #           en: Our references
  - name: docs-quickstart
    url: /docs-quickstart
    sections: 
      - name: setup
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-setup-en.md
          en: ./texts/documentation/docs-setup-en.md
  - name: docs-integration
    url: /docs-integration
    sections: 
      - name: integration
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-integration-en.md
          en: ./texts/documentation/docs-integration-en.md
  - name: docs-gitfile
    url: /docs-gitfile
    sections: 
      - name: docs-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-gitfile-en.md
          en: ./texts/documentation/docs-gitfile-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-gitfile.md
          en: ./texts/documentation/docs-params/param-gitfile.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-usertoken.md
          en: ./texts/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-git
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-usertoken-notes-git.md
          en: ./texts/documentation/docs-params/param-usertoken-notes-git.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-options/option-global.md
          en: ./texts/documentation/docs-options/option-global.md
      - name: docs-option-gitfile-md
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-md.md
          en: ./texts/documentation/docs-options/option-gitfile-md.md
      - name: docs-option-gitfile-json
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-json.md
          en: ./texts/documentation/docs-options/option-gitfile-json.md
      - name: docs-option-gitfile-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-options/option-gitfile-csv.md
          en: ./texts/documentation/docs-options/option-gitfile-csv.md
  - name: docs-explowiki
    url: /docs-explowiki
    sections: 
      - name: docs-explowiki
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-explowiki-en.md
          en: ./texts/documentation/docs-explowiki-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-wikilist
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-wikilist.md
          en: ./texts/documentation/docs-params/param-wikilist.md
      - name: docs-param-wikipages
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-wikipages.md
          en: ./texts/documentation/docs-params/param-wikipages.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-usertoken.md
          en: ./texts/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-mediawiki
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-usertoken-notes-mediawiki.md
          en: ./texts/documentation/docs-params/param-usertoken-notes-mediawiki.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-options/option-global.md
          en: ./texts/documentation/docs-options/option-global.md
  - name: docs-multi-files
    url: /docs-multi-files
    sections: 
      - name: docs-multi-files
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-multi-files-en.md
          en: ./texts/documentation/docs-multi-files-en.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-title.md
          en: ./texts/documentation/docs-params/param-title.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-locale.md
          en: ./texts/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
        files:
          fr: ./texts/documentation/docs-params/param-debug.md
          en: ./texts/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          # columns-divider: h1
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
