---
routes: 

  # LANDING
  - name: home
    url: /
    options:
      description:
        fr: Page d'accueil de la documentation de Datami
        en: Homepage for Datami documentation
      keywords:
        fr: [ accueil, landing ]
        en: [ homepage, landing ]
      # hero: true
    sections:
      - name: landing
        component: TextComponent
        options:
          columns-size: full
          # hero: true
          # custom-class: my-6
        files:
          fr: ./texts/fr/landing/landing.md
          en: ./texts/en/landing/landing.md
      - name: landing-before-after
        component: TextComponent
        options:
          columns-size: full
          # hero: true
          # custom-class: my-6
        files:
          fr: ./texts/fr/landing/landing-before-after.md
          en: ./texts/en/landing/landing-before-after.md
      - name: landing-features
        component: TextComponent
        options:
          columns-size: full
          # hero: true
          # custom-class: my-6
        files:
          fr: ./texts/fr/landing/landing-features.md
          en: ./texts/en/landing/landing-features.md
      # - name: logo
      #   component: TextComponent
      #   options:
      #     columns-size: '5'
      #   files:
      #     fr: ./texts/international/logo-gitribute.md
      #     en: ./texts/international/logo-gitribute.md
      # - name: catchphrase
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/fr/landing/catchphrase.md
      #     en: ./texts/en/landing/catchphrase.md
      # - name: btns
      #   component: ButtonsComponent
      #   options:
      #     columns-size: three-quarters
      #     buttons-size: half
      #     buttons:
      #       - link: /why-datami
      #         icon-left: help-circle
      #         rounded: true
      #         label:
      #           fr: Pourquoi utiliser Datami
      #           en: Why you need Datami
            # - link: /tutorial-overview
            #   icon-left: school
            #   rounded: true
            #   label: 
            #     fr: Tutoriels
            #     en: Tutorials
            # - link: /docs-widgets-overview
            #   icon-left: book-open-variant
            #   rounded: true
            #   label: 
            #     fr: Documentation
            #     en: Widgets' docs
            # - link: https://gitlab.com/multi-coop/datami
            #  icon-left: gitlab
            #  rounded: true
            #  label: 
            #    fr: Code source
            #    en: Source code
      # - name: logo-multi
      #   component: TextComponent
      #   options:
      #     columns-size: full
      #   files:
      #     fr: ./texts/fr/landing/landing-multi.md
      #     en: ./texts/en/landing/landing-multi.md
      # - name: more-intro
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/international/more.md
      #     en: ./texts/international/more.md
      - name: intro
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/fr/landing/landing-intro.md
          en: ./texts/en/landing/landing-intro.md
      # - name: more-simulator
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/international/more.md
      #     en: ./texts/international/more.md
      # - name: landing-gitribute-cooptech
      #   component: HtmlComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/fr/gallery/demo-cooptech.md
      #     en: ./texts/en/gallery/demo-cooptech.md
      - name: datami-cooptech
        component: WidgetComponent
        options:
          columns-size: two-thirds
          js: 
            - href: https://datami-widget.multi.coop/js/app.js
          css: 
            - href: https://datami-widget.multi.coop/css/app.css
          html: |
            <datami-file
              title="Liste des coopératives de la tech en France"
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
      # - name: more-clients
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/international/more.md
      #     en: ./texts/international/more.md
      - name: clients
        component: TextComponent
        options:
          columns-size: full
          custom-class: my-6 py-6
        files:
          fr: ./texts/fr/landing/landing-clients.md
          en: ./texts/en/landing/landing-clients.md
      # - name: more-outro
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/international/more.md
      #     en: ./texts/international/more.md
      # - name: outro
      #   component: TextComponent
      #   options:
      #     columns-size: two-thirds
      #   files:
      #     fr: ./texts/fr/landing/landing-outro.md
      #     en: ./texts/en/landing/landing-outro.md
      # - name: more-why
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #   files:
      #     fr: ./texts/international/more.md
      #     en: ./texts/international/more.md
      - name: btn-to-contact
        component: ButtonsComponent
        options:
          columns-size: three-quarters
          custom-class: my-6
          buttons-size: one-third
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Contactez-nous
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md

  # WHAT IS DATAMI
  - name: why-datami
    url: /why-datami
    options:
      summary: true
      contrib: true
      name:
        fr: Pourquoi Datami ?
        en: Why Datami ?
      description:
        fr: Pourquoi nous développons le logiciel libre Datami ?
        en: Why are we developping the free software Datami ?
      keywords:
        fr: [ pourquoi, simplifier, aider, ouvrir, réduire les coûts, open data ]
        en: [ why, simplify, help, open, cheap, open data ]
    sections:
      # - name: logo
      #   component: TextComponent
      #   options:
      #     columns-size: '2 is-hidden-touch'
      #     not-in-menu: true
      #   files:
      #     fr: ./texts/international/logo-gitribute-bis.md
      #     en: ./texts/international/logo-gitribute-bis.md
      - name: why-intro
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/why-datami/why-datami.md
          en: ./texts/en/why-datami/why-datami.md
      # - name: why-flashback
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     name:
      #       fr: Flashback
      #       en: Flashback
      #   files:
      #     fr: ./texts/fr/why-datami/why-datami-flashback.md
      #     en: ./texts/en/why-datami/why-datami-flashback.md
      - name: why-intro-easy
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: 😅 · Simplififier la contribution ouverte
            en: 😅 · Make open contribution easier 
        files:
          fr: ./texts/fr/why-datami/why-datami-easy.md
          en: ./texts/en/why-datami/why-datami-easy.md
      - name: why-open
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: 🔧 · Aider les organisation à ouvrir leurs données
            en: 🔧 · Help organizations opening data
        files:
          fr: ./texts/fr/why-datami/why-datami-open.md
          en: ./texts/en/why-datami/why-datami-open.md
      - name: why-costs
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: 💸 · Réduire le coût de l'open data
            en: 💸 · Reduce the cost of open data
        files:
          fr: ./texts/fr/why-datami/why-datami-costs.md
          en: ./texts/en/why-datami/why-datami-costs.md
      - name: why-quality
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: ✨ · Faire de l'open data de qualité
            en: ✨ · Make quality open data
        files:
          fr: ./texts/fr/why-datami/why-datami-quality.md
          en: ./texts/en/why-datami/why-datami-quality.md
      - name: why-quality-schemas
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Data & schémas de données
            en: Data & schemas
        files:
          fr: ./texts/fr/why-datami/why-datami-quality-schemas.md
          en: ./texts/en/why-datami/why-datami-quality-schemas.md
      - name: why-quality-consolidation
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Consolidation de données
            en: Data consolidation
        files:
          fr: ./texts/fr/why-datami/why-datami-quality-consolidation.md
          en: ./texts/en/why-datami/why-datami-quality-consolidation.md
      # - name: logo
      #   component: TextComponent
      #   options:
      #     columns-size: '5'
      #     not-in-menu: true
      #   files:
      #     fr: ./texts/international/logo-gitribute.md
      #     en: ./texts/international/logo-gitribute.md
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
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: main-features
    url: /main-features
    options:
      summary: true
      contrib: true
      name:
        fr: Principales fonctionnalités
        en: Main features
      description:
        fr: Les fonctionnalités principales et innovantes de nos widgets
        en: The widgets' main original features
      keywords:
        fr: [ éditer, contribuer, partager, adapter, visualiser, dataviz ]
        en: [ edit, contribute, share, adapt, visualise, dataviz ]
    sections: 
      - name: main-features
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/main-features/main-features.md
          en: ./texts/en/main-features/main-features.md
      - name: main-features-edit
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Éditer & contribuer online
            en: Edit & contribute online
        files:
          fr: ./texts/fr/main-features/main-features-edit.md
          en: ./texts/en/main-features/main-features-edit.md
      - name: main-features-share
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Partager vos jeux de données
            en: Share your datasets
        files:
          fr: ./texts/fr/main-features/main-features-share.md
          en: ./texts/en/main-features/main-features-share.md
      - name: main-features-adapt
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Adapter les widgets à vos besoins
            en: Adapt the widgets to your needs
        files:
          fr: ./texts/fr/main-features/main-features-adapt.md
          en: ./texts/en/main-features/main-features-adapt.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: business-model
    url: /business-model
    options:
      # hero: true
      summary: true
      contrib: true
      name:
        fr: "100% libre & gratuit"
        en: "100% free"
      description:
        fr: Datami est entièrement open source
        en: Datami is entirely free & open source
      keywords:
        fr: [ open source, free ]
        en: [ open  source, free ]
    sections: 
      - name: business-model
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/business-model/business-model.md
          en: ./texts/en/business-model/business-model.md
      - name: business-model-no_trap
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Pas de piège, juste open source
            en: No trap, just open source
        files:
          fr: ./texts/fr/business-model/business-model-no_trap.md
          en: ./texts/en/business-model/business-model-no_trap.md
      # - name: business-model-idea
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     depth: 1
      #     name:
      #       fr: Une idée, et la preuve rapide que ça fonctionne
      #       en: An idea, and the quick proof it could technically work
      #   files:
      #     fr: ./texts/fr/business-model/business-model-idea.md
      #     en: ./texts/en/business-model/business-model-idea.md
      # - name: business-model-usecases
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     depth: 1
      #     name:
      #       fr: Des vrais cas d'usage
      #       en: Real use cases
      #   files:
      #     fr: ./texts/fr/business-model/business-model-usecases.md
      #     en: ./texts/en/business-model/business-model-usecases.md
      # - name: business-model-mutualize
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     depth: 1
      #     name:
      #       fr: Mutualiser & converger sur une feuille de route
      #       en: Mutualize & converge with the roadmap 
      #   files:
      #     fr: ./texts/fr/business-model/business-model-mutualize.md
      #     en: ./texts/en/business-model/business-model-mutualize.md
      # - name: business-model-valorize
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     depth: 1
      #     name:
      #       fr: Valoriser l'expertise, pas le code
      #       en: Valorize the expertise, not the code
      #   files:
      #     fr: ./texts/fr/business-model/business-model-valorize.md
      #     en: ./texts/en/business-model/business-model-valorize.md
      - name: clients
        component: TextComponent
        options:
          columns-size: full
          name:
            fr: Ils soutiennent Datami
            en: They support Datami
        files:
          fr: ./texts/fr/landing/landing-clients.md
          en: ./texts/en/landing/landing-clients.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  
  # BENCHMARK
  - name: benchmark
    url: /benchmark
    options:
      contrib: true
      summary: true
      name:
        fr: Benchmark
        en: Benchmark
      description:
        fr: Comparaisons des solutions équivalentes
        en: Comparison between similar solutions
      keywords:
        fr: [ benchmark, no code ]
        en: [ benchmark, no code ]
    sections: 
      - name: benchmark-head
        component: TextComponent
        options:
          columns-size: full
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/benchmark/fr/benchmark-head.md
          en: ./texts/benchmark/en/benchmark-head.md
      - name: benchmark-comparisons
        component: TextComponent
        options:
          columns-size: full
          name:
            fr: Compairisons
            en: Comparisons
        files:
          fr: ./texts/benchmark/fr/benchmark-comparisons.md
          en: ./texts/benchmark/en/benchmark-comparisons.md
      - name: benchmark-comparisons-open
        component: TextComponent
        options:
          columns-size: full
          depth: 1
          name:
            fr: Solutions open source
            en: Open source solutions
        files:
          fr: ./texts/benchmark/benchmark-comparisons-open.md
          en: ./texts/benchmark/benchmark-comparisons-open.md
      - name: benchmark-comparisons-proprietary
        component: TextComponent
        options:
          columns-size: full
          depth: 1
          name:
            fr: Solutions propriétaires
            en: Proprietary solutions
        files:
          fr: ./texts/benchmark/benchmark-comparisons-proprietary.md
          en: ./texts/benchmark/benchmark-comparisons-proprietary.md
      - name: benchmark-solutions
        component: TextComponent
        options:
          columns-size: full
          name:
            fr: Solutions
            en: Solutions
        files:
          fr: ./texts/benchmark/fr/benchmark-solutions.md
          en: ./texts/benchmark/en/benchmark-solutions.md
      - name: benchmark-data
        component: DataGrid
        options:
          columns-size: full
          depth: 1
          name:
            fr: Listing
            en: Grid list
        files:
          fr: ./texts/benchmark/benchmark-data.md
          en: ./texts/benchmark/benchmark-data.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md

  # TUTORIAL
  - name: tutorial-overview
    url: /tutorial-overview
    options:
      summary: true
      contrib: true
      name:
        fr: Panorama des tutoriels
        en: Tutorials overview
      description:
        fr: Liste des tutoriels de prise en main des widgets
        en: Tutorials list to learn how to use widgets
      keywords:
        fr: [ tutoriel, panorama ]
        en: [ tutorial, overview ]
    sections: 
      - name: tutorial-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/tutorial/tutorial-overview.md
          en: ./texts/en/tutorial/tutorial-overview.md
      - name: tutorial-overview-actions
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Voir les informations du document
            en: View document's informations
        files:
          fr: ./texts/fr/tutorial/tutorial-overview-actions.md
          en: ./texts/en/tutorial/tutorial-overview-actions.md
      - name: tutorial-overview-edition
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Édition & vues d'un document
            en: Edition & document's views
        files:
          fr: ./texts/fr/tutorial/tutorial-overview-edition.md
          en: ./texts/en/tutorial/tutorial-overview-edition.md
      - name: tutorial-overview-contribution
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Contribuer à un document
            en: Contribute to a document
        files:
          fr: ./texts/fr/tutorial/tutorial-overview-contribution.md
          en: ./texts/en/tutorial/tutorial-overview-contribution.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: tutorial-actions
    url: /tutorial-actions
    options:
      summary: true
      contrib: true
      name:
        fr: Informations sur le document
        en: Document's infos
      description:
        fr: voir les informations sur un document de données
        en: check the informations about a data file
      keywords:
        fr: [ tutoriel, infos, fichier, dataset ]
        en: [ tutorial, infos, file, dataset ]
    sections: 
      - name: tutorial-actions
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/tutorial/tutorial-actions.md
          en: ./texts/en/tutorial/tutorial-actions.md
      - name: tutorial-actions-file-infos
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Informations sur le fichier
            en: File's informations
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-file-infos.md
          en: ./texts/en/tutorial/tutorial-actions-file-infos.md
      - name: tutorial-actions-user-options
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Options de l'utilisateur
            en: User's options
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options.md
          en: ./texts/en/tutorial/tutorial-actions-user-options.md
      - name: tutorial-actions-user-options-reload
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Recharger le fichier source
            en: Reload the source file
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-reload.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-reload.md
      - name: tutorial-actions-user-options-download
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Télécharger le fichier
            en: Download the file
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-download.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-download.md
      - name: tutorial-actions-user-options-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Changer le token utilisateur
            en: Change your user token
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-usertoken.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-usertoken.md
      - name: tutorial-actions-user-options-branches
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Vérifier vos branches
            en: Check your branches
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-branches.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-branches.md
      - name: tutorial-actions-user-options-copy
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Copier le widget 
            en: Copy the widget
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-copy.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-copy.md
      - name: tutorial-actions-user-options-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Changer de langue
            en: Change the language
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-locale.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-locale.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: tutorial-views
    url: /tutorial-views
    options:
      summary: true
      contrib: true
      name:
        fr: Vues d'un document
        en: Document's views
      description:
        fr: Les modes de visualisation d'un document de données
        en: The visualisation mode for a dataset
      keywords:
        fr: [ tutoriel, vues, datavisualisation ]
        en: [ tutorial, views, datavisualisation ]
    sections:
      - name: tutorial-actions-change-modes
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Les modes de vue
            en: The view modes
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-change-modes.md
          en: ./texts/en/tutorial/tutorial-actions-change-modes.md
      - name: tutorial-actions-edit-modes
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Changer le mode de "vue-édition"
            en: Switch the "edit-view" modes
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-edit-modes.md
          en: ./texts/en/tutorial/tutorial-actions-edit-modes.md
      - name: tutorial-actions-edit-modes-preview
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Le mode "Prévisualisation"
            en: The "Preview" mode
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-edit-modes-preview.md
          en: ./texts/en/tutorial/tutorial-actions-edit-modes-preview.md
      - name: tutorial-actions-edit-modes-edit
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Le mode "Édition"
            en: The "Edit" mode
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-edit-modes-edit.md
          en: ./texts/en/tutorial/tutorial-actions-edit-modes-edit.md
      - name: tutorial-actions-edit-modes-diff
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Le mode "Comparaison"
            en: The "Diff" mode
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-edit-modes-diff.md
          en: ./texts/en/tutorial/tutorial-actions-edit-modes-diff.md
      - name: tutorial-actions-cards_view
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Vue "cartes"
            en: Cards view
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-cards_view.md
          en: ./texts/en/tutorial/tutorial-actions-cards_view.md
      - name: tutorial-actions-search_filters
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Rechercher et filtrer
            en: Search and filter
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-search_filters.md
          en: ./texts/en/tutorial/tutorial-actions-search_filters.md
      - name: tutorial-actions-search
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Recherche textuelle
            en: Fulltext search
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-search.md
          en: ./texts/en/tutorial/tutorial-actions-search.md
      - name: tutorial-actions-filters
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Filtres
            en: Filters
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-filters.md
          en: ./texts/en/tutorial/tutorial-actions-filters.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: tutorial-edition
    url: /tutorial-edition
    options:
      summary: true
      contrib: true
      name:
        fr: Éditer un document
        en: Edit a document
      description:
        fr: Les options d'édition d'un document
        en: How to edit a document
      keywords:
        fr: [ tutoriel, éditer ]
        en: [ tutorial, edit ]
    sections: 
      - name: edition
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/tutorial/tutorial-edition.md
          en: ./texts/en/tutorial/tutorial-edition.md
      - name: edition-md
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Éditer un fichier markdown
            en: Edit a markdown file
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-md.md
          en: ./texts/en/tutorial/tutorial-edition-edit-md.md
      - name: edition-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Éditer un fichier CSV
            en: Edit a CSV file
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-csv.md
          en: ./texts/en/tutorial/tutorial-edition-edit-csv.md
      - name: edition-csv-fields
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Champs d'un tableur
            en: Table fields
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-csv-fields.md
          en: ./texts/en/tutorial/tutorial-edition-edit-csv-fields.md
      - name: edition-csv-rows
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Opérations usuelles sur les lignes
            en: Common rows operations
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-csv-rows.md
          en: ./texts/en/tutorial/tutorial-edition-edit-csv-rows.md
      - name: edition-csv-consolidation_field
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Champ de consolidation
            en: Consolidation field
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-csv-consolidation_field.md
          en: ./texts/en/tutorial/tutorial-edition-edit-csv-consolidation_field.md
      - name: edition-json
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Éditer un fichier JSON
            en: Edit a JSON file
        files:
          fr: ./texts/fr/tutorial/tutorial-edition-edit-json.md
          en: ./texts/en/tutorial/tutorial-edition-edit-json.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: tutorial-contribution
    url: /tutorial-contribution
    options:
      summary: true
      contrib: true
      name:
        fr: Contribuer à un document
        en: Contribute to a document
      description:
        fr: Comment contribuer sur un même fichier et dataset
        en: How to contribute on the same document or file
      keywords:
        fr: [ tutoriel, contribuer, éditer ]
        en: [ tutorial, contribute, edit ]
    sections: 
      # - name: contribution
      #   component: TextComponent
      #   options:
      #     columns-size: three-quarters
      #     name:
      #       fr: Introduction
      #       en: Introduction
      #   files:
      #     fr: ./texts/fr/tutorial/tutorial-contribution.md
      #     en: ./texts/en/tutorial/tutorial-contribution.md
      - name: contribution-send
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/tutorial/tutorial-contribution-send.md
          en: ./texts/en/tutorial/tutorial-contribution-send.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: integration
    url: /integration
    options:
      # hero: true
      contrib: true
      summary: true
      name:
        fr: Intégration de Datami dans un site web
        en: Datami's integration in a website
      description:
        fr: Comment intégrer Datami facilement dans votre site web
        en: How to easily integrate Datami within your website
      keywords:
        fr: [ tutoriel, intégration, widget ]
        en: [ tutorial, integration, widget ]
    sections: 
      - name: integration
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/integration/integration.md
          en: ./texts/en/integration/integration.md
      - name: integration-example
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Exemple
            en: Example
        files:
          fr: ./texts/fr/integration/integration-example.md
          en: ./texts/en/integration/integration-example.md
      - name: integration-no_panic
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Pas de panique !
            en: Do not panic !
        files:
          fr: ./texts/fr/integration/integration-no_panic.md
          en: ./texts/en/integration/integration-no_panic.md
      - name: integration-dependencies
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Dépendances
            en: Dependencies
        files:
          fr: ./texts/fr/integration/integration-dependencies.md
          en: ./texts/en/integration/integration-dependencies.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          custom-class: mt-6
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: integration-wordpress
    url: /integration-wordpress
    options:
      # hero: true
      contrib: true
      summary: true
      name:
        fr: Intégration dans Wordpress
        en: Wordpress integration
      description:
        fr: Intégrer un widget Datami dans Wordpress 
        en: Integrate a Datami widget in a wordpress website
      keywords:
        fr: [ tutoriel, intégration, Wordpress ]
        en: [ tutorial, integration, Wordpress ]
    sections:
      - name: integration
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/integration-wordpress/wordpress.md
          en: ./texts/en/integration-wordpress/wordpress.md
      - name: login
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: S'authentifier dans le backoffice
            en: Log to the backoffice
        files:
          fr: ./texts/fr/integration-wordpress/wordpress-login.md
          en: ./texts/en/integration-wordpress/wordpress-login.md
      - name: back-office
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Créer une nouvelle page
            en: Create a new page
        files:
          fr: ./texts/fr/integration-wordpress/wordpress-admin.md
          en: ./texts/en/integration-wordpress/wordpress-admin.md
      - name: edit-01
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Passer en mode "Editeur de code"
            en: Switch to "Code editor"
        files:
          fr: ./texts/fr/integration-wordpress/wordpress-edit-code.md
          en: ./texts/en/integration-wordpress/wordpress-edit-code.md
      - name: tutorial-actions-user-options-copy
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Copier le widget
            en: Copy the widget
        files:
          fr: ./texts/fr/tutorial/tutorial-actions-user-options-copy.md
          en: ./texts/en/tutorial/tutorial-actions-user-options-copy.md
      - name: edit-03
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Coller le widget
            en: Paste the widget
        files:
          fr: ./texts/fr/integration-wordpress/wordpress-edit-paste.md
          en: ./texts/en/integration-wordpress/wordpress-edit-paste.md
      - name: preview
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Prévisualiser le résultat
            en: Preview the result
        files:
          fr: ./texts/fr/integration-wordpress/wordpress-preview.md
          en: ./texts/en/integration-wordpress/wordpress-preview.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          custom-class: mt-6
          buttons-size: half
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md

  # DOCUMENTATION - TECH
  - name: install
    url: /install
    options:
      summary: true
      contrib: true
      name:
        fr: Stratégies d'installation
        en: Installation strategies
      description:
        fr: Comment installer Datami ?
        en: How to install Datami ?
      keywords:
        fr: [ documentation, installation, réutiliser, adapter ]
        en: [ documentation, install, reuse, adapt ]
    sections: 
      - name: installation
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/installation/installation.md
          en: ./texts/en/installation/installation.md
      - name: installation-reuse
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Réutiliser des widgets
            en: Reuse some widgets
        files:
          fr: ./texts/fr/installation/installation-reuse.md
          en: ./texts/en/installation/installation-reuse.md
      - name: installation-adapt
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Adapter Datami à votre site
            en: Adapt Datami for your website
        files:
          fr: ./texts/fr/installation/installation-adapt.md
          en: ./texts/en/installation/installation-adapt.md
      - name: installation-instance
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Installer votre instance
            en: Install your instance
        files:
          fr: ./texts/fr/installation/installation-instance.md
          en: ./texts/en/installation/installation-instance.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          custom-class: mt-6
          buttons-size: half
          buttons:
            - link: https://gitlab.com/multi-coop/datami
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
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: quickstart-developpers
    url: /quickstart-developpers
    options:
      contrib: true
      summary: true
      name:
        fr: Quickstart pour les développeurs
        en: Quickstart for developpers
      description:
        fr: Guide rapide d'installation pour les développeurs
        en: Quick installation guide for developpers 
      keywords:
        fr: [ documentation, installation, développeurs ]
        en: [ documentation, install, developpers ]
    sections: 
      - name: intro
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/quickstart/introduction.md
          en: ./texts/en/quickstart/introduction.md
      - name: setup
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Setup
            en: Setup
        files:
          fr: ./texts/fr/quickstart/setup.md
          en: ./texts/en/quickstart/setup.md
      - name: env-file
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Le fichier `env`
            en: The `env` file
        files:
          fr: ./texts/fr/quickstart/env-file.md
          en: ./texts/en/quickstart/env-file.md
      - name: local-dev
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Développement local
            en: Local development
        files:
          fr: ./texts/fr/quickstart/local-dev.md
          en: ./texts/en/quickstart/local-dev.md
      - name: production
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Production
            en: Production
        files:
          fr: ./texts/fr/quickstart/production.md
          en: ./texts/en/quickstart/production.md
      - name: linting
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Linting
            en: Linting
        files:
          fr: ./texts/fr/quickstart/linting.md
          en: ./texts/en/quickstart/linting.md
      - name: unit-tests
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Tests unitaires
            en: Unit tests
        files:
          fr: ./texts/fr/quickstart/unit-tests.md
          en: ./texts/en/quickstart/unit-tests.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          custom-class: mt-6
          buttons-size: half
          buttons:
            - link: https://gitlab.com/multi-coop/datami
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
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: software
    url: /software
    options:
      contrib: true
      summary: true
      name:
        fr: Infos sur le logiciel
        en: Software informations
      description:
        fr: Informations sur les librairies utilisées
        en: Infos about the software
      keywords:
        fr: [ documentation, stack, roadmap, contribution, open source ]
        en: [ documentation, stack, roadmap, contribution, open source ]
    sections: 
      - name: docs-licence
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Licence
            en: Licence
        files:
          fr: ./texts/fr/software/licence.md
          en: ./texts/en/software/licence.md
      - name: docs-stack
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Stack
            en: Stack
        files:
          fr: ./texts/fr/software/stack.md
          en: ./texts/en/software/stack.md
      - name: roadmap
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Feuille de route
            en: Roadmap
        files:
          fr: ./texts/fr/software/roadmap.md
          en: ./texts/en/software/roadmap.md
      - name: roadmap-poc
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: POC
            en: POC
        files:
          fr: ./texts/fr/software/roadmap-poc.md
          en: ./texts/en/software/roadmap-poc.md
      - name: roadmap-mvp
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: MVP
            en: MVP
        files:
          fr: ./texts/fr/software/roadmap-mvp.md
          en: ./texts/en/software/roadmap-mvp.md
      - name: contributing
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Contribuer à la documentation
            en: Contributing to the docs
        files:
          fr: ./texts/fr/software/contributing.md
          en: ./texts/en/software/contributing.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            # - link: /roadmap
            #   icon-left: map-search-outline
            #   rounded: true
            #   label: 
            #     fr: Roadmap
            #     en: Roadmap
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
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md

  # DOCUMENTATION - WIDGETS
  - name: docs-widgets-overview
    url: /docs-widgets-overview
    options:
      summary: true
      contrib: true
      name:
        fr: Panorama des widgets
        en: Widgets overview
      description:
        fr: Liste des widgets propulsés par Datami
        en: List of widgets powered by Datami
      keywords:
        fr: [ documentation, gitfile, multi-files, explowiki ]
        en: [ documentation, gitfile, multi-files, explowiki ]
    sections:
      - name: docs-widgets-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Introduction
            en: Introduction
        files:
          fr: ./texts/fr/documentation/docs-widgets-overview.md
          en: ./texts/en/documentation/docs-widgets-overview.md
      - name: docs-widgets-overview-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le widget "gitfile"
            en: The "gitfile" widget
        files:
          fr: ./texts/fr/documentation/docs-gitfile.md
          en: ./texts/en/documentation/docs-gitfile.md
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
                fr: Widget Gitfile
                en: Gitfile widget
      - name: docs-widgets-overview-multifiles
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le widget "multi-files"
            en: The "multi-files" widget
        files:
          fr: ./texts/fr/documentation/docs-multi-files.md
          en: ./texts/en/documentation/docs-multi-files.md
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
                fr: Widget Multi-files
                en: Multi-files widget
      - name: docs-widgets-overview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le widget "explowiki"
            en: The "explowiki" widget
        files:
          fr: ./texts/fr/documentation/docs-explowiki.md
          en: ./texts/en/documentation/docs-explowiki.md
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
                fr: Widget Explowiki
                en: Explowiki widget
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: docs-gitfile
    url: /docs-gitfile
    options:
      summary: true
      contrib: true
      name:
        fr: Le widget "gitfile"
        en: The "gitfile" widget
      description:
        fr: Détails de configuration du widget gitfile
        en: Configuration details of the gitfile widget
      keywords:
        fr: [ documentation, config, gitfile ]
        en: [ documentation, config, gitfile ]
    sections: 
      - name: docs-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Présentation
            en: Presentation
        files:
          fr: ./texts/fr/documentation/docs-gitfile.md
          en: ./texts/en/documentation/docs-gitfile.md
      - name: docs-gitfile-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Structure
            en: Structure
        files:
          fr: ./texts/fr/documentation/docs-gitfile-structure.md
          en: ./texts/en/documentation/docs-gitfile-structure.md
      - name: docs-gitfile-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Exemple
            en: Example
        files:
          fr: ./texts/fr/documentation/docs-gitfile-structure-example.md
          en: ./texts/en/documentation/docs-gitfile-structure-example.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Paramètres
            en: Parameters
        files:
          fr: ./texts/fr/documentation/docs-params/params.md
          en: ./texts/en/documentation/docs-params/params.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "title"
            en: The "title" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-title.md
          en: ./texts/en/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "height"
            en: The "height" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-height.md
          en: ./texts/en/documentation/docs-params/param-height.md
      - name: docs-param-gitfile
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "gitfile"
            en: The "gitfile" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-gitfile.md
          en: ./texts/en/documentation/docs-params/param-gitfile.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "usertoken"
            en: The "usertoken" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-usertoken.md
          en: ./texts/en/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-git
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Notes à propos du paramètre "usertoken"
            en: Notes about the "usertoken" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-usertoken-notes-git.md
          en: ./texts/en/documentation/docs-params/param-usertoken-notes-git.md
      - name: docs-param-onlypreview
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "onlypreview"
            en: The "onlypreview" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-onlypreview.md
          en: ./texts/en/documentation/docs-params/param-onlypreview.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "locale"
            en: The "locale" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-locale.md
          en: ./texts/en/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "debug"
            en: The "debug" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-debug.md
          en: ./texts/en/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "options"
            en: The "options" parameter
        files:
          fr: ./texts/fr/documentation/docs-options/option-global.md
          en: ./texts/en/documentation/docs-options/option-global.md
      - name: docs-option-gitfile-csv
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Les clés des "options" pour fichiers tabulaires
            en: The "options" keys for table files
        files:
          fr: ./texts/fr/documentation/docs-options/option-gitfile-csv.md
          en: ./texts/en/documentation/docs-options/option-gitfile-csv.md
      - name: docs-option-gitfile-custom_props
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Fichier de propriétés custom pour fichiers tabulaires
            en: Custom properties file for table files
        files:
          fr: ./texts/fr/documentation/docs-custom-props/props-custom_props.md
          en: ./texts/en/documentation/docs-custom-props/props-custom_props.md
      - name: docs-option-gitfile-json
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: The "options" keys for json files
            en: The "options" keys for json files
        files:
          fr: ./texts/fr/documentation/docs-options/option-gitfile-json.md
          en: ./texts/en/documentation/docs-options/option-gitfile-json.md
      - name: docs-option-gitfile-md
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Les clés des "options" pour fichiers md
            en: The "options" keys for md files
        files:
          fr: ./texts/fr/documentation/docs-options/option-gitfile-md.md
          en: ./texts/en/documentation/docs-options/option-gitfile-md.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md
  - name: docs-explowiki
    url: /docs-explowiki
    options:
      summary: true
      contrib: true
      name:
        fr: Le widget "explowiki"
        en: The "explowiki" widget
      description:
        fr: Détails de configuration du widget explowiki
        en: Configuration details of the explowiki widget
      keywords:
        fr: [ documentation, config, explowiki ]
        en: [ documentation, config, explowiki ]
    sections: 
      - name: docs-explowiki
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Présentation
            en: Presentation
        files:
          fr: ./texts/fr/documentation/docs-explowiki.md
          en: ./texts/en/documentation/docs-explowiki.md
      - name: docs-explowiki-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Structure
            en: Structure
        files:
          fr: ./texts/fr/documentation/docs-explowiki-structure.md
          en: ./texts/en/documentation/docs-explowiki-structure.md
      - name: docs-explowiki-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Exemple
            en: Example
        files:
          fr: ./texts/fr/documentation/docs-explowiki-structure-example.md
          en: ./texts/en/documentation/docs-explowiki-structure-example.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Paramètres
            en: Parameters
        files:
          fr: ./texts/fr/documentation/docs-params/params.md
          en: ./texts/en/documentation/docs-params/params.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "title"
            en: The "title" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-title.md
          en: ./texts/en/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "height"
            en: The "height" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-height.md
          en: ./texts/en/documentation/docs-params/param-height.md
      - name: docs-param-wikilist
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "wikilist"
            en: The "wikilist" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-wikilist.md
          en: ./texts/en/documentation/docs-params/param-wikilist.md
      - name: docs-param-wikipages
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "wikipages"
            en: The "wikipages" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-wikipages.md
          en: ./texts/en/documentation/docs-params/param-wikipages.md
      - name: docs-param-usertoken
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "usertoken"
            en: The "usertoken" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-usertoken.md
          en: ./texts/en/documentation/docs-params/param-usertoken.md
      - name: docs-param-usertoken-notes-mediawiki
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Notes à propos du paramètre "usertoken"
            en: Notes about the "usertoken" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-usertoken-notes-mediawiki.md
          en: ./texts/en/documentation/docs-params/param-usertoken-notes-mediawiki.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "locale"
            en: The "locale" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-locale.md
          en: ./texts/en/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "debug"
            en: The "debug" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-debug.md
          en: ./texts/en/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "options"
            en: The "options" parameter
        files:
          fr: ./texts/fr/documentation/docs-options/option-global.md
          en: ./texts/en/documentation/docs-options/option-global.md
      - name: docs-option-explowiki-table
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Les clés "options" pour des données wiki
            en: The "options" keys for wiki data
        files:
          fr: ./texts/fr/documentation/docs-options/option-explowiki-table.md
          en: ./texts/en/documentation/docs-options/option-explowiki-table.md
      - name: docs-option-explowiki-custom_props
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Fichier de propriétés custom pour données wiki 
            en: Custom properties file for wiki data
        files:
          fr: ./texts/fr/documentation/docs-custom-props/props-custom_props.md
          en: ./texts/en/documentation/docs-custom-props/props-custom_props.md
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
        fr: Le widget "multi-files"
        en: The "multi-files" widget
      description:
        fr: Détails de configuration du widget multi-files
        en: Configuration details of the multi-files widget
      keywords:
        fr: [ documentation, config, multi-files ]
        en: [ documentation, config, multi-files ]
    sections: 
      - name: docs-multi-files
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Présentation
            en: Presentation
        files:
          fr: ./texts/fr/documentation/docs-multi-files.md
          en: ./texts/en/documentation/docs-multi-files.md
      - name: docs-multi-files-structure
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Structure
            en: Structure
        files:
          fr: ./texts/fr/documentation/docs-multi-files-structure.md
          en: ./texts/en/documentation/docs-multi-files-structure.md
      - name: docs-multi-files-structure-example
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: Exemple
            en: Example
        files:
          fr: ./texts/fr/documentation/docs-multi-files-structure-example.md
          en: ./texts/en/documentation/docs-multi-files-structure-example.md
      - name: docs-params
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Paramètres
            en: Parameters
        files:
          fr: ./texts/fr/documentation/docs-params/params.md
          en: ./texts/en/documentation/docs-params/params.md
      - name: docs-param-title
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "title"
            en: The "title" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-title.md
          en: ./texts/en/documentation/docs-params/param-title.md
      - name: docs-param-height
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "height"
            en: The "height" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-height.md
          en: ./texts/en/documentation/docs-params/param-height.md
      - name: docs-param-gitfiles
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "gitfiles"
            en: The "gitfiles" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-gitfiles.md
          en: ./texts/en/documentation/docs-params/param-gitfiles.md
      - name: docs-param-locale
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "locale"
            en: The "locale" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-locale.md
          en: ./texts/en/documentation/docs-params/param-locale.md
      - name: docs-param-debug
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "debug"
            en: The "debug" parameter
        files:
          fr: ./texts/fr/documentation/docs-params/param-debug.md
          en: ./texts/en/documentation/docs-params/param-debug.md
      - name: docs-option-global
        component: TextComponent
        options:
          columns-size: three-quarters
          name:
            fr: Le paramètre "options"
            en: The "options" parameter
        files:
          fr: ./texts/fr/documentation/docs-options/option-global.md
          en: ./texts/en/documentation/docs-options/option-global.md
      - name: docs-option-multifiles
        component: TextComponent
        options:
          columns-size: three-quarters
          depth: 1
          name:
            fr: The "options" keys for multi-files
            en: The "options" keys for multi-files
        files:
          fr: ./texts/fr/documentation/docs-options/option-multifiles.md
          en: ./texts/en/documentation/docs-options/option-multifiles.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
      - name: logo-multi
        component: TextComponent
        options:
          columns-size: full
          custom-class: mt-6
          not-in-menu: true
        files:
          fr: ./texts/fr/landing/landing-multi.md
          en: ./texts/en/landing/landing-multi.md

  # STANDARD ROUTES
  - name: Contact
    url: /contact
    options:
      hero: true
      name:
        fr: Contactez-nous
        en: Contact us
      description:
        fr: Contactez-nous pour plus d'infos
        en: Contact us for more infos
      keywords:
        fr: [ contact, mail ]
        en: [ contact, mail ]
    sections: 
      - name: Contact
        component: TextComponent
        options:
          columns-size: three-quarters
          # custom-class: mt-6
          # columns-divider: h1
        files:
          fr: ./texts/fr/contact/contact-head.md
          en: ./texts/en/contact/contact-head.md
  - name: legal
    url: /legal
    options:
      name:
        fr: Mentions légales
        en: Legal
      description:
        fr: Mentions légales
        en: Legal mentions
      keywords:
        fr: [ contact, légal ]
        en: [ contact, legal ]
    sections: 
      # - name: data
      #   component: TextDataComponent
      #   files:
      #     fr: ./texts/fr/contact/legal-data.md
      - name: legal-text
        component: TextComponent
        files:
          fr: ./texts/fr/contact/legal-mentions.md
          en: ./texts/en/contact/legal-mentions.md
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

  # GALLERY - HTML
  - name: demo-cooptech
    url: /demo-cooptech
    options:
      contrib: true
      name:
        fr: Démo Cooptech
        en: Demo Cooptech
      description:
        fr: Démonstrateur avec les données de Cooptech
        en: Demonstrator with Cooptech dataset
      keywords:
        fr: [ démo, cooptech ]
        en: [ demo, cooptech ]
    sections:
      - name: demo-gitribute-cooptech
        component: HtmlComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/gallery/demo-cooptech.md
          en: ./texts/gallery/demo-cooptech.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: demo-odf-observatoire
    url: /demo-odf-observatoire
    options:
      contrib: true
      name:
        fr: Démo Open Data France | Observatoire
        en: Demo Open Data France | Observatory
      description:
        fr: Démonstrateur avec les données de l'Observatoire d'Open Data France
        en: Demonstrator with Open Data France Observatory dataset
      keywords:
        fr: [ démo, ODF ]
        en: [ demo, ODF ]
    sections:
      - name: demo-gitribute-odf-observatoire
        component: HtmlComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/gallery/demo-odf-observatoire.md
          en: ./texts/gallery/demo-odf-observatoire.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: demo-odf-ressources
    url: /demo-odf-ressources
    options:
      contrib: true
      name:
        fr: Démo Open Data France | Ressources
        en: Demo Open Data France | Ressources
      description:
        fr: Démonstrateur avec les données des Ressources d'Open Data France
        en: Demonstrator with Open Data France Ressources dataset
      keywords:
        fr: [ démo, ODF ]
        en: [ demo, ODF ]
    sections:
      - name: demo-gitribute-odf-ressources
        component: HtmlComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/gallery/demo-odf-ressources.md
          en: ./texts/gallery/demo-odf-ressources.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: demo-fabmob
    url: /demo-fabmob
    options:
      contrib: true
      name:
        fr: Démo Fabmob
        en: Demo Fabmob
      description:
        fr: Démonstrateur avec les données wiki de la Fabrique des mobilités
        en: Demonstrator with Fabmob wiki dataset
      keywords:
        fr: [ démo, fabmob ]
        en: [ demo, fabmob ]
    sections:
      - name: demo-gitribute-fabmob
        component: HtmlComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/gallery/demo-fabmob.md
          en: ./texts/gallery/demo-fabmob.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us
  - name: demo-aac
    url: /demo-aac
    options:
      contrib: true
      name:
        fr: Démo appel à communs de l'ADEME
        en: Demo AAC ADEME
      description:
        fr: Démonstrateur avec les données wiki de l'appel à communs de l'ADEME
        en: Demonstrator with ADEME-AAC wiki dataset
      keywords:
        fr: [ démo, ADEME ]
        en: [ demo, ADEME ]
    sections:
      - name: demo-gitribute-aac
        component: HtmlComponent
        options:
          columns-size: three-quarters
        files:
          fr: ./texts/gallery/demo-aac.md
          en: ./texts/gallery/demo-aac.md
      - name: Contact
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          custom-class: mt-6
          buttons:
            - link: /contact
              icon-left: email
              rounded: true
              label: 
                fr: Nous contacter
                en: Contact us

  # GALLERY - WIDGET / DEPRECATED
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
            <datami-multi-files 
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
            ]'></datami-multi-files>
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
            <datami-file
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
            </datami-file>
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
            <datami-file
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
            <datami-explowiki
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
              }' title="gitribute for explowiki - fabmob :)" locale="fr"></datami-explowiki>
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


  # BLOG
  # - name: blog
  #   url: /blog
  #   options:
  #     name:
  #       fr: Espace de blog
  #       en: Blog section
  #     description:
  #       fr: Espace de blog du projet Datami
  #       en: Blog section of Datami
  #     keywords:
  #       fr: [ blog ]
  #       en: [ blog ]
  #   sections: 
  #     - name: head
  #       component: TextComponent
  #       options:
  #         columns-size: two-thirds
  #       files:
  #         fr: ./texts/blog/fr/blog-head.md
  #         en: ./texts/blog/en/blog-head.md
  #     - name: data
  #       component: DataGrid
  #       files:
  #         fr: ./texts/blog/fr/blog-data.md
  #         en: ./texts/blog/en/blog-data.md
--- 
