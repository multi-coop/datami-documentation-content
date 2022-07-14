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
  - file: ./texts/en/benchmark/solutions/gitribute.md
  - file: ./texts/en/benchmark/solutions/data-patch.md
  - file: ./texts/en/benchmark/solutions/gis.md
  - file: ./texts/en/benchmark/solutions/nocodb.md
  - file: ./texts/en/benchmark/solutions/framacalc.md
  - file: ./texts/en/benchmark/solutions/libreoffice.md
  - file: ./texts/en/benchmark/solutions/koumoul.md
  - file: ./texts/en/benchmark/solutions/mediawiki.md
  - file: ./texts/en/benchmark/solutions/semapps.md
  - file: ./texts/en/benchmark/solutions/ckan.md
  # propriteary
  - file: ./texts/en/benchmark/solutions/airtable.md
  - file: ./texts/en/benchmark/solutions/kantree.md
  - file: ./texts/en/benchmark/solutions/notion.md
  - file: ./texts/en/benchmark/solutions/coda.md
  - file: ./texts/en/benchmark/solutions/googlesheet.md
  - file: ./texts/en/benchmark/solutions/excel.md
  - file: ./texts/en/benchmark/solutions/ods.md


dict:
  open:
    en: Open source
  type:
    en: Project type
  description:
    en: Description
  approach:
    en: Approach
  stage:
    en: Stage
  technos:
    en: Technos
  code:
    en: Code
---
