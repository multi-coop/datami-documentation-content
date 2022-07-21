---
type: solutions

options:
  title-key: name
  images-key: images
  images-ratio: 7by4
  columns-size: one-third
  shuffle: true

  card-modal: true
  card-modal-config:
    full-screen: true
    column-left: false
    column-right: 
      default-text: description
      infos-texts: 
        - period
        - type
        - approach
      tabs:
        - infos
        - gallery 
        - links 
      images-gallery: true

  miniature-keys: 
    # - technos
    - stage

  texts-keys: 
    - description 
    - period
    - type
    - approach

  links-keys: 
    - code

  tags-keys: 
    - key: open
      color: primary
    - key: stage
      color: light
    - key: technos
      color: light
  filters: 
    activate: true
    items: 
      - name: open
      # - name: technos
      - name: stage

items: 
  # open source
  - file: ./texts/benchmark/solutions/gitribute.md
  - file: ./texts/benchmark/solutions/data-patch.md
  - file: ./texts/benchmark/solutions/gis.md
  - file: ./texts/benchmark/solutions/nocodb.md
  - file: ./texts/benchmark/solutions/framacalc.md
  - file: ./texts/benchmark/solutions/libreoffice.md
  - file: ./texts/benchmark/solutions/koumoul.md
  - file: ./texts/benchmark/solutions/mediawiki.md
  - file: ./texts/benchmark/solutions/semapps.md
  - file: ./texts/benchmark/solutions/ckan.md
  # propriteary
  - file: ./texts/benchmark/solutions/airtable.md
  - file: ./texts/benchmark/solutions/kantree.md
  - file: ./texts/benchmark/solutions/notion.md
  - file: ./texts/benchmark/solutions/coda.md
  - file: ./texts/benchmark/solutions/googlesheet.md
  - file: ./texts/benchmark/solutions/excel.md
  - file: ./texts/benchmark/solutions/ods.md


dict:
  open:
    fr: Open source
    en: Open source
  type:
    fr: Project type
    en: Project type
  description:
    fr: Description
    en: Description
  approach:
    fr: Approach
    en: Approach
  stage:
    fr: Stage
    en: Stage
  technos:
    fr: Technos
    en: Technos
  code:
    fr: Code
    en: Code
---
