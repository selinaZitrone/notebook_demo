---
title: <% tp.file.title %>
date: 
startTime: 
endTime: 
attendees: []
location: 
tags:
  - meeting
topic:
---

# 👩‍👩‍👧‍👦 Meeting name
## 💼 Agenda



## 🌞 Summary
```dataviewjs
function callout(text, type) {
    const allText = `> [!${type}]\n` + text;
    const lines = allText.split('\n');
    return lines.join('\n> ') + '\n'
}

const query = `
short mode
path includes ${dv.current().file.path}
# you can add any number of extra Tasks instructions, for example:
# group by heading
`;

dv.paragraph(callout('```tasks\n' + query + '\n```', 'todo'));
```
> [!Summary]
> - [ ] write Summary

## 📒 Meeting notes


