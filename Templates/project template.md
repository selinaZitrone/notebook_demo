---
start: null
completed: null
tags: project
collaborators: null
description: null
state: null
publication: null
priority: null
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
table 
	dateformat(date, "yyyy-MM-dd") as date, topic, attendees, summary
from [[#this.file.name]] AND #meeting
sort date DESC
```
## ↪ Mentions 
```dataview
table 
	dateformat(date, "yyyy-MM-dd") as date, tags
from [[#this.file.name]] AND -#meeting
sort date DESC
```

