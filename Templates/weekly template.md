---
tag: weeklyReview
week: {{date:ww}} 
---
# Week {{date:ww}}

## 🏔 Goals
- Goal 1
- Goal 2
- Goal 3

## 🐾 Tasks
```tasks
(due before {{friday:gggg-MM-DD}}) OR (due {{friday:gggg-MM-DD}})
not done
group by due
path does not include 01_Journal/Weekly
short mode
```


## 📜 Weekly review 
### 😊 What went well
- x
- x
- x
### 😞 What do I want to improve
- x
- x
- x

### 🌴 Daily log files of the week
```base
views:
  - type: table
    name: Default view
    order:
      - file.name
    filters:
      and:
        - file.hasTag("dailyLog")
        - date >= date("{{monday:YYYY-MM-DD}}")
        - date <= date("{{friday:YYYY-MM-DD}}")
display:
  file.name: Name
```
