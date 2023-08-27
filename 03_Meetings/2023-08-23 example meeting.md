---
title: 2023-08-23 example meeting
date: 2023-08-23
startTime: 08:00
endTime: 09:00
attendees:
  - Jane Doe
  - John Doe
location: New York
tags:
  - meeting
  - project_A
topic: Planing meeting
---
# 👩‍👩‍👧‍👦  Example Meeting
## 💼 Agenda
- Talk about next project steps
- Define next goals
- [ ] Invite Hans-Jochen for the meeting 📅 2023-08-22
- [x] Prepare example event 📅 2023-08-22 ✅ 2023-08-27
- [x] Make coffee for the example event 📅 2023-08-23 ✅ 2023-08-23

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
> - Lorem ipsum dolor sit amet.
> - consetetur sadipscing elitr

## 📒 Meeting notes
- Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 
- At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. 
- [ ] Talk to Ferdinand about next steps 📅 2023-08-24
- [ ] Send notes from meeting to all collaborators 📅 2023-08-23

- Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. 


- [ ] think about the meetings outcome