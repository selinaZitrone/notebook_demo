---
date: {{date}}
tags: dailyLog
---
# {{date:dddd, D MMMM, YYYY}}

## 🧑‍🤝‍🧑 Meetings 
```dataview
TABLE
  topic AS "topic",
  startTime AS "start",
  endTime AS "end"
FROM #meeting
WHERE date =  date("{{date}}") OR contains(file.name, "{{date}}")
SORT start DESC
```

## 🐾 Tasks

#### From the past
```tasks
not done
happens before {{date}}
short mode
```

#### Today
```tasks
path does not include 01_Journal/Daily
happens on {{date}}
short mode
group by folder
```

## 🏴‍☠ Log


## 🗺 Changed files

```dataview
LIST 
	dateformat(file.mtime, "HH:mm") 
WHERE striptime(file.mtime) = this.file.day WHERE file.name != this.file.name 
SORT file.mtime DESC
```


