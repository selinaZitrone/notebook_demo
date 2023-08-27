---
topic: 
date: <% tp.file.creation_date("YYYY-MM-DD") %>
tags:
  - note
  - project_name
---

Before you start writing your note remember:
- set link to project file below
- set project name as a tag in the YAML header/properties
# 🦋 <% tp.file.title %>
project::

## 🧭 Summary 
```dataviewjs
function callout(text, type) {
    const allText = `> [!${type}]\n` + text;
    const lines = allText.split('\n');
    return lines.join('\n> ') + '\n'
}

const query = `
short mode
path includes ${dv.current().file.path}
`;

dv.paragraph(callout('```tasks\n' + query + '\n```', 'todo'));
```
> [!Summary]
> - [ ] write Summary


## 📒 Notes