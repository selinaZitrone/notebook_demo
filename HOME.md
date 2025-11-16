# HOME

## 🏡 Vault info
- **Vault owner**: *add*
- **Vault purpose**: *write something*
- **Vault origin**: This vault is based on a [Demo Vault](https://github.com/selinaZitrone/notebook_demo) by S. Baldauf and A. Lewerentz.

## 📈 Vault statistics
- File Count: `$=dv.pages().length`
- Daily Journal Entries: `$=dv.pages('"01_Journal/Daily"').length`
- Weekly Journal Entries: `$=dv.pages('"01_Journal/Weekly"').length`
- Number of Zettel:  `$=dv.pages('"05_Zettelkasten"').length`

## 📊 Projects
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.tags.contains("project")
        - file.folder != "Templates"
    order:
      - file.name
      - collaborators
      - description
      - state
    columnSize:
      file.name: 149
      note.collaborators: 148
      note.description: 297

```

## ✅ Open tasks without due date
*Comment: This section collects all your open tasks without a due date from your vault.* 

```tasks
not done
no due date
short mode
group by folder
path does not include Templates/
#path does not include 01_Journal
```
