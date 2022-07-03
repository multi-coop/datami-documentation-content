---
type: network

options:
  title-key: title
  subtitle-key: subtitle
  illustration-key: logo
  illustration-height: 50px
  columns-size: full
  has-readmore: false

  list: true
  shuffle: true

  card-modal: false
  card-modal-config:
    full-screen: true
    column-left: false
    column-right: true
    infos-texts: 
      - type

  tags-keys: 
    - key: type
      color: light
    - key: tags
      color: info

  filters: 
    activate: true
    items: 
      - name: type
      - name: tags

items:
  - file: ./texts/network/items/codeurs-en-liberte.md
  - file: ./texts/network/items/data-for-good.md
  - file: ./texts/network/items/eig.md
  - file: ./texts/network/items/fairness.md
  - file: ./texts/network/items/latitudes.md
  - file: ./texts/network/items/mednum.md
  - file: ./texts/network/items/urscop-idf.md
  - file: ./texts/network/items/scopyleft.md
  - file: ./texts/network/items/ut7.md
  - file: ./texts/network/items/ping.md
  - file: ./texts/network/items/open-data-france.md
  - file: ./texts/network/items/open-source-politics.md
  - file: ./texts/network/items/code-for-france.md
  - file: ./texts/network/items/leon.md
  - file: ./texts/network/items/april.md
  - file: ./texts/network/items/aful.md
  - file: ./texts/network/items/framasoft.md
  - file: ./texts/network/items/cooptech.md
  - file: ./texts/network/items/open-heroines.md
  - file: ./texts/network/items/la-banquiz.md
  - file: ./texts/network/items/fabmob.md
  - file: ./texts/network/items/ademe-resilience.md
  # - file: ./texts/network/items/usages-communs.md

dict:
  type:
    fr: Type de structure
    en: Structure type
  tags:
    fr: tags
    en: tags
---
