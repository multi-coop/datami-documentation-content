---
type: blog-posts

options:
  title-key: title
  columns-size: one-third
  has-readmore: true

  # shuffle: true

  card-modal: true
  card-modal-config:
    full-screen: true
    column-left: false
    column-right: true
    infos-texts: 
      - author
      - created

  miniature-keys: 
    - author
    - created
    - tags

  tags-keys: 
    - key: tags
      color: primary

  filters: 
    activate: true
    items: 
      - name: tags

items:
  - file: ./texts/blog/fr/posts/main-ideas.md
  - file: ./texts/blog/fr/posts/flashback.md
  - file: ./texts/blog/fr/posts/business-model-idea.md
  - file: ./texts/blog/fr/posts/contribution.md
  - file: ./texts/blog/fr/posts/how-it-works.md
  - file: ./texts/blog/fr/posts/contribution-what.md
  - file: ./texts/blog/fr/posts/everything-looks-like-excel.md
  - file: ./texts/blog/fr/posts/sketches.md

dict:
  created:
    fr: Date de publication
  author:
    fr: Auteur
  tags:
    fr: tags
---
