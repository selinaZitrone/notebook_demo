# Vault of *add your name*

## 🏡 Vault info
- Purpose of my vault: *write something*
-   〽️ Stats
    -   File Count: `$=dv.pages().length`
    -   Daily Journal Entries: `$=dv.pages('"01_Journal/Daily"').length`
    -   Weekly Journal Entries: `$=dv.pages('"01_Journal/Weekly"').length`

## 📊 Projects
```dataview
TABLE 
	collaborators, 
	description,
	state
FROM #project AND -"Templates"
```


## ✅ Open tasks without due date
*Comment: This file collects all your open tasks without a due date from your vault except from the Journal folder. The idea is that you can visit this page if you don't know what to do or if you need an overview about your tasks.*

```tasks
not done
no due date
short mode
group by folder
path does not include Templates/
path does not include 01_Journal
```
