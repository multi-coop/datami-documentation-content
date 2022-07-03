---
type: jobs

options:
  title-key: title
  columns-size: one-third
  has-readmore: false
  # readmore-divider: h1
  
  # card-modal: true
  # card-modal-config:
  #   full-screen: true
  #   column-left: false
  #   column-right: true
  #   infos-texts: 
  #     - post_date

  miniature-keys: 
    # - post_date
    - job_status
    - tags

  tags-keys: 
    - key: job_status
      color: primary
    - key: tags
      color: info

  filters: 
    activate: true
    items: 
      - name: job_status
      - name: tags
    
items:
  - file: ./texts/jobs/posts/jobs-post-spontaneous-fr.md
  - file: ./texts/jobs/posts/jobs-post-02-fr.md
  - file: ./texts/jobs/posts/jobs-post-01-fr.md

dict:
  job_status: 
    fr: statut
    en: status
  tags:
    fr: tags
    en: tags
  post_date:
    fr: Date de publication
    en: Publication date
---
