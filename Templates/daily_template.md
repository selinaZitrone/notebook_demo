---
Date: {{date}}
Tags: dailyLog
---

# {{date:dddd, D MMMM, YYYY}}

<< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>| Yesterday ]] | [[<% tp.date.now("gggg-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>]] | [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>| Tomorrow ]] >>

## 🧑‍🤝‍🧑 Events & meetings 
```dataview
TABLE
  title AS "topic",
  startTime AS "start",
  endTime AS "end"
FROM -"1_Journal/Daily"
WHERE contains(file.name, "{{date}}")
SORT start DESC
```

## 🐾 Tasks

#### From The past
```tasks
not done
happens before {{date}}
short mode
```

#### Today
```tasks
path does not include 1_Laborbuch/1_Daily
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


