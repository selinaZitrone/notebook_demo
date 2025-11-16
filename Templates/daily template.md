---
date: {{date}}
tags: dailyLog
---
# {{date:dddd, D MMMM, YYYY}}

## 🧑‍🤝‍🧑 Meetings 
```base
views:
  - type: table
    name: Default view
    order:
      - file.name
      - topic
      - startTime
      - endTime
    sort:
      - column: start
        direction: desc
    columnSize:
      note.topic: 359
      note.startTime: 76
    filters:
      and:
        - file.hasTag("meeting")
        - or:
            - date == date(this.file.name)
            - file.name.contains(date(this.file.name).toString())
display:
  file.name: Name
  topic: topic
  startTime: start
  endTime: end

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


