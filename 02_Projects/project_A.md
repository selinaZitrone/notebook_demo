---
name: project_A
start: 2023-08-01
completed: 
tags:
  - project
collaborators:
  - Johanna
  - Rolf
description: something meaningful
state: ongoing
---
# project_A

## 🦸‍♀ Description
Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.

## 🗃 Resources 
- e.g. link to shared google drive document
- or link to canvas files [[brainstorming.canvas|brainstorming]]

## 👷‍♀ All tasks within project 
```dataviewjs
const tag = "#project_A"
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



## ↪ Notes & Mentions 
```dataview
table 
	dateformat(date, "yyyy-MM-dd") as date, tags
FROM [[#this.file.name]] AND -#meeting
SORT date DESC
```


## 🏅 Activity 
> [!Success]
> - Paper published in Nature
> - Poster prize at ECEM 23 conference

