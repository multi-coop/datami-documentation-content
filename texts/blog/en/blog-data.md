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
  - file: ./texts/blog/en/posts/main-ideas.md
  - file: ./texts/blog/en/posts/flashback.md
  - file: ./texts/blog/en/posts/business-model-idea.md
  - file: ./texts/blog/en/posts/contribution.md
  - file: ./texts/blog/en/posts/how-it-works.md
  - file: ./texts/blog/en/posts/contribution-what.md
  - file: ./texts/blog/en/posts/everything-looks-like-excel.md
  - file: ./texts/blog/en/posts/sketches.md

dict:
  created:
    en: Publication date
  author:
    en: Author
  tags:
    en: tags
---
