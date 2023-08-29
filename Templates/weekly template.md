---
tag: weeklyReview
week: {{date:ww}} 
---
<< [[<% tp.date.now("gggg-[W]ww", -1, tp.file.title, "gggg-[W]ww") %>|last week]] | [[<% tp.date.now("gggg-[W]ww", 8, tp.file.title, "gggg-[W]ww") %>|next week]] >> 
# 🚀 Week {{date:ww}}

## 🏔 Goals
- Goal 1
- Goal 2
- Goal 3

## 🐾 Tasks
```tasks
(due before {{friday:gggg-MM-DD}}) OR (due {{friday:gggg-MM-DD}})
not done
group by due
path does not include 1_Laborbuch/2_Weekly
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
```dataview
list
FROM #dailyLog
WHERE date >= date("{{monday:YYYY-MM-DD}}") AND date <= date("{{friday:YYYY-MM-DD}}")
```

