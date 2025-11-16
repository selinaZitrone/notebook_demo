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

## 📒 Notes & Mentions 
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


## 🏅 Activity & Success
> [!Success]
> - x

