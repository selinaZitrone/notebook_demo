---
tag: weeklyReview
week: {{date:ww}} 
---
<< [[<% tp.date.now("gggg-[W]ww", -1, tp.file.title, "gggg-[W]ww") %>|last week]] | [[<% tp.date.now("gggg-[W]ww", 8, tp.file.title, "gggg-[W]ww") %>|next week]] >> 
# 🚀 Start of the week

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
- [ ] Do weekly review 📅 {{friday:gggg-MM-DD}}

# 🌞 End of the week

## 📜 Weekly review and wrap up
- [ ] Check all daily files of last week and re-date undone tasks
- [ ] Check if weekly tasks are done
- [ ] Write weekly review
- [ ] Add weekly goals and notes for next week
- [ ] Check [[ALL OPEN TASKS]] and plan tasks for next week

### What went well
- x
- x
- x
### What do I want to improve
- x
- x
- x

### 🌴 Daily log files of the week
```dataview
TABLE date
FROM #dailyLog
WHERE date >= date("{{monday:YYYY-MM-DD}}") AND date <= date("{{friday:YYYY-MM-DD}}")
```

