---
name: project_A
start: 2025-08-01
completed:
tags:
  - project
collaborators:
  - Johanna
  - Rolf
description: something meaningful
state: ongoing
---
# My cool project A

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
```base
views:
  - type: table
	name: Default view
	order:
	  - file.name
	  - date
	  - attendees
	  - topic
	sort:
	  - column: date
	    direction: desc
	filters:
	  and:
	    - file.hasTag("meeting")
	    - or:
	        - file.hasTag(this.file.name)
	        - file.hasLink(this.file)
```

## ↪ Notes & Mentions 
```base
views:
  - type: table
	name: Default view
	order:
	  - file.name
	  - date
	  - tags
	sort:
	  - column: date
	    direction: desc
	filters:
	  and:
	    - not:
	        - file.hasTag("meeting")
	    - or:
	        - file.hasTag(this.file.name)
	        - file.hasLink(this.file)
```


## 🏅 Activity 
> [!Success]
> - Paper published in Nature
> - Poster prize at ECEM 23 conference

