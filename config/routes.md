---
routes: 

  # LANDING
  - name: home 
    url: /
    options:
      hero: true
    sections: 
      - name: logo
        component: LogoAnimated
        options:
          columns-size: two-thirds
          no-translation: true
        files:
          fr: ./texts/landing/landing-head-fr.md
          en: ./texts/landing/landing-head-fr.md
      - name: head
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/landing/catchphrase-fr.md
          en: ./texts/landing/catchphrase-en.md
      - name: btn-to-offer-products
        component: ButtonsComponent
        options:
          columns-size: full
          buttons-size: full
          buttons: 
            - link: /offer
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Documentation
                en: Documentation
  
  # WHO ARE WE
  - name: what
    url: /what-gitribute-does
    options:
      hero: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/why-gitribute/what-fr.md
          en: ./texts/why-gitribute/what-en.md
      # - name: btn-to-team
      #   component: ButtonsComponent
      #   options:
      #     columns-size: full
      #     buttons-size: half
      #     buttons: 
      #       - link: /team
      #         icon-left: arrow-right-bold
      #         rounded: true
      #         label: 
      #           fr: Découvrez l'équipe
      #           en: Discover the team
      #       - link: /references
      #         icon-left: arrow-right-bold
      #         rounded: true
      #         label: 
      #           fr: Nos références
      #           en: Our references

  - name: why
    url: /why-gitribute
    options: [ menu ]
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/origin-fr.md
          en: ./texts/why-gitribute/origin-en.md
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/why-gitribute/roadmap-fr.md
          en: ./texts/why-gitribute/roadmap-en.md

  - name: team 
    url: /team
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/team/team-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/team/team-data.md
      - name: btn-to-jobs
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: full
          custom-classes: mt-6
          buttons: 
            - link: /jobs
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Nos offres d'emploi
                en: Our job offers

  # OFFER
  - name: documentation
    url: /documentation
    sections: 
      - name: offer-head
        component: TextComponent
        options:
          columns-size: two-thirds
          # columns-divider: h1
        files:
          fr: ./texts/offer/offer-head-fr.md
      - name: btn-to-products
        component: ButtonsComponent
        options:
          columns-size: two-thirds
          buttons-size: half
          buttons: 
            - link: /products
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Nos produits open source
                en: Our open source products
            - link: /references
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Nos références
                en: Our references

  - name: offer-temp
    url: /offer-temp
    sections: 
      - name: offer-temp
        component: TextComponent
        options:
          columns-size: full
        files:
          fr: ./texts/offer/offer-temp-fr.md

  - name: products
    url: /products
    sections: 
      - name: products-head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/references/products-head-fr.md
      - name: products-data
        component: DataGrid
        files:
          fr: ./texts/references/products-data.md
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
      - name: refs-data
        component: DataGrid
        files:
          fr: ./texts/references/references-data.md

  - name: infos
    url: /infos
    options:
      hero: true
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: full
          columns-divider: h1
        files:
          fr: ./texts/contact/infos-head-fr.md
      - name: btn-to-jobs
        component: ButtonsComponent
        options:
          columns-size: full
          buttons-size: full
          buttons: 
            - link: /contribute
              icon-left: arrow-right-bold
              rounded: true
              label: 
                fr: Contribuer
                en: Contribute

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
      - name: data
        component: DataGrid
        files:
          fr: ./texts/jobs/jobs-data.md


  - name: blog
    url: /blog
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/blog/blog-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/blog/blog-data.md

  - name: network
    url: /network
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/network/network-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/network/network-data.md

  - name: ressources
    url: /ressources
    sections: 
      - name: head
        component: TextComponent
        options:
          columns-size: two-thirds
        files:
          fr: ./texts/ressources/ressources-head-fr.md
      - name: data
        component: DataGrid
        files:
          fr: ./texts/ressources/ressources-data.md

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
