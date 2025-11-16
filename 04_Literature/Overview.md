# 📚 Literature

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
```
