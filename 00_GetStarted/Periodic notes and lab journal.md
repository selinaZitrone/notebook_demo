# 📆 Periodic notes and lab journal
*Plugins used*: Calendar, Templater, Periodic Notes, Tasks

The idea of periodic notes is that you use them to track your goals, tasks and work on a daily/weekly basis. In this workflow, we use two templates:
- [[daily template]]: Create this file every day to get an overview of your tasks and meetings on that day, but also to take notes.
- [[weekly template]]: Create this file every week to plan ahead what you want to focus on and get done in that week. Can also be used to review the week after it's over.
## Create a periodic note
To create a periodic note for a day/week, first locate the calendar in your notebook (probably either the bottom left corner or in the right side bar). By clicking on a date or week a daily/weekly note is created automatically from the correct template and some information is already filled out. You can find the newly created notes in the folder `01_Journal/Daily|Weekly`. 
## Structure of a daily note (e.g. [[2023-08-23]])
- **Header**: On top, the header automatically contains the date and weekday.
- **🧑‍🤝‍🧑Meetings**: The dataview query in this section automatically looks for meetings that happen on that day. If you want to see the structure of the query, just click on the `</>` symbol in the top right corner of the meeting table. You can use the link in the table to go directly to the meeting file.
- **🐾Tasks**: A section with a task query to automatically find tasks from the past that were forgotten (task due date is over) and tasks that happen today. Here you can also add other tasks for that day manually. When a task is done, just check the checkbox.
- **🏴‍☠Log**: A log section that you can use to log your activities that day, take notes, link other files etc.
- **🗺Changed files**: A list of Obsidian files that you changed that day. This list is automatically compiled with the dataview plugin. Can be useful to easily see the files you worked on that day.
## Structure of a weekly note (e.g. [[2023-W34]])
- **⛰Goals**: Write down your goals for the week.
- **🐾Tasks**: A section that automatically pulls all the tasks for this week into the file. You can manually add other tasks below.
- **📜Weekly review**: Space for reviewing the week and planning ahead the next week.
## A word on tasks
When a task is done, you can check the checkbox. Here is an example of an open and a closed task:
- [ ] Describe what "tasks" are 📅 2023-08-28 
- [x] Describe what done tasks are 📅 2022-12-22 ✅ 2022-12-22
You can also use the Hotkey `Ctrl/Cmd + Alt/Option + T` to edit tasks.

In the file [[HOME]] you can find a list of all the open tasks without due date in your vault. You can periodically check this file to see which tasks you might have forgotten.

