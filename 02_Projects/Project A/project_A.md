---
start: 2023-08-01
completed: null
tags: project
collaborators: Jane Doe, John Doe
description: Modelling biodiversity in a forest
state: ongoing
name: project_A
---

# Name 

## 🦸‍♀ Description

Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
## 👷‍♀ All tasks within project 
```tasks
not done
short mode
path includes 02_Projects/Project A 
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

