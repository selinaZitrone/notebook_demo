---
start: null
completed: null
tags: project
collaborators: null
description: null
state: ""
name: ""
---
# Name 

## 🦸‍♀ Description

## 👷‍♀ All tasks within project 
```tasks
not done
short mode
path includes <% tp.file.folder(true) %> 
```

## 🏅 Activity 

## 🧑‍🤝‍🧑 Meetings
```dataview
TABLE 
	dateformat(date, "yyyy-MM-dd") as date, attendees, summary
FROM #meeting
WHERE contains(tags, this.file.name)
SORT date DESC
```
## ↪ Mentions 
```dataview
table 
	dateformat(date, "yyyy-MM-dd") as date, tags
FROM -#meeting
WHERE contains(tags, this.file.name)
SORT date DESC
```

