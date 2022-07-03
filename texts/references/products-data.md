---
type: products

options:
  title-key: name
  images-key: images
  images-ratio: 7by4
  columns-size: one-third

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
        - resources
      tabs:
        - infos
        - gallery 
        - links 
      images-gallery: true

  miniature-keys: 
    - technos
    - clients

  texts-keys: 
    - description 
    - period
    - type
    - approach
    - resources

  links-keys: 
    - refs 
    - code

  tags-keys: 
    - key: clients
      color: primary
    - key: technos
      color: light
  filters: 
    activate: true
    items: 
      - name: technos
      - name: clients

items: 
  - file: ./texts/references/projects/data-patch.md
  - file: ./texts/references/projects/barometre-action-publique.md
  # - file: ./texts/references/projects/africartes.md
  # - file: ./texts/references/projects/aides-entreprises.md
  # - file: ./texts/references/projects/open-mobility-indicators.md
  # - file: ./texts/references/projects/parcours-entree-dans-emploi.md
  # - file: ./texts/references/projects/play-with-transitions.md
  # - file: ./texts/references/projects/digital-transport-for-africa.md
  # - file: ./texts/references/projects/observatoire-open-data-des-territoires.md
  - file: ./texts/references/projects/apiviz.md
  - file: ./texts/references/projects/solidata.md
  - file: ./texts/references/projects/open-scraper.md
  - file: ./texts/references/projects/validata.md
  # - file: ./texts/references/projects/dbnomics.md
  # - file: ./texts/references/projects/open-fisca.md
  # - file: ./texts/references/projects/synapse.md
  # - file: ./texts/references/projects/hydroviz.md
  # - file: ./texts/references/projects/libviz.md


dict:
  clients:
    fr: Clients
    en: Clients
  period:
    fr: Période
    en: Period
  type:
    fr: Type de projet
    en: Project type
  description:
    fr: Description
    en: Description
  approach:
    fr: Approche et contraintes
    en: Approach
  resources:
    fr: Ressources
    en: Resources
  technos:
    fr: Technologies
    en: Technos
  refs:
    fr: Références
    en: References
  code:
    fr: Code source
    en: Code
---
