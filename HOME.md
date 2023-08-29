# Home file

## 🏡 Vault info
- Vault owner: *add*
- Vault purpose: *write something*
- Vault Statistics: 
    - File Count: `$=dv.pages().length`
    - Daily Journal Entries: `$=dv.pages('"01_Journal/Daily"').length`
    - Weekly Journal Entries: `$=dv.pages('"01_Journal/Weekly"').length`
    - Number of Zettel:  `$=dv.pages('"05_Zettelkasten"').length`

## 📊 Projects
```dataview
TABLE 
	collaborators, 
	description,
	state
FROM #project AND -"Templates"
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
