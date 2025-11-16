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

```base
filters:
  and:
    - file.name != this.file.name
    - file.mtime.date() == date(this.file.name)
views:
  - type: list
    name: Changed Today
    sort:
      - property: file.mtime
        direction: DESC
    properties:
      file.name: {}
      formula.time:
        formula: formatDate(file.mtime, "HH:mm")

```


