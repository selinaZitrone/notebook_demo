# 📚 Literature notes

```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.folder == "04_Literature/library"
    order:
      - file.name
      - journal
      - title
      - authors
      - year
    sort:
      - property: year
        direction: ASC
    columnSize:
      file.name: 100
      note.journal: 109
      note.title: 244
      note.authors: 348

```
