---
name: <% tp.file.title %>
start: <% tp.file.creation_date("YYYY-MM-DD") %>
completed: 
tags:
  - project
collaborators: []
description: 
state: ""
---
# <% tp.file.title %>

## 🦸‍♀ Description


## 🗃 Resources 


## 👷‍♀ All tasks within project 
```dataviewjs
const tag = "#<% tp.file.title %>"
const query = `
	  not done
	  ${"(path includes " + dv.pagePaths(tag).join(') OR (path includes ') + ")"}
	  short mode`;
	  dv.paragraph('```tasks\n' + query + '\n```');
```

## 🧑‍🤝‍🧑 Meetings
```dataview
TABLE 
	dateformat(date, "yyyy-MM-dd") as date, attendees, topic
FROM #meeting
WHERE contains(tags, this.file.name)
SORT date DESC
```



## 📒 Notes & Mentions 
```dataview
table 
	dateformat(date, "yyyy-MM-dd") as date, tags
FROM [[#this.file.name]] AND -#meeting
SORT date DESC
```


## 🏅 Activity & Success
> [!Success]
> - x

