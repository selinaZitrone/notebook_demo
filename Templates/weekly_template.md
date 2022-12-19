---
tag: weeklyReview
week:  {{date:ww}} 
---

# 🚀 Start of the week

## 🏔 Goals

## 🐾 Tasks

- [ ] Do weekly review 📅 {{friday:gggg-MM-DD}}

```tasks
(due before {{friday:gggg-MM-DD}}) OR (due {{friday:gggg-MM-DD}})
not done
group by due
path does not include 1_Laborbuch/2_Weekly
short mode
```


#### optional

# 🌞 End of the week

## 📜 Weekly review and wrap up

- [ ] Fill in YAML header (Labmeeting, etc.)
- [ ] Check all daily files of last week and re-date undone tasks
- [ ] Check if weekly tasks are done
- [ ] Write weekly review
- [ ] Add weekly goals and notes for next week
- [ ] Check [[Open-Tasks]] and plan tasks for next week
- [ ] Update [[HOME]] Page
- [ ] Check that in [[README#Orphan files]] only future events exist
- [ ] Check if any todo tags open

### 🌴 Daily log files of the week
```dataview
TABLE date, file.size
FROM #dailyLog AND "1_Laborbuch"
WHERE date >= date("{{monday:YYYY-MM-DD}}") AND date <= date("{{friday:YYYY-MM-DD}}")
```
### 🐘 What went well
### 💪 What do I want to improve
### 🐌 Mood
