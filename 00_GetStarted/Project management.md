# 📊 Project management
*Plugins used*: Templater, Tasks

The idea of this workflow is that for every project, you have one main project file in the folder `02_Projects`. This file is your entry point into the project, holds the most important info of your project and links to other project notes and meetings.
## Start a new project

Create a new project file in the `02_Projects` folder and apply the [[project template]] to it (see [[Create note from template]] for instructions). 

>[!warning] Caution 
>In our workflow, we create a project tag for every project. The tag is called like the project file (e.g. project_A and #project_A ). Therefore do not use any white space in your project file name. You can e.g. concatenate the file name using underscores.

The new project file can now be filled with life (see [[project_A|this example file]]). In the project file, you can write down tasks (if you give the tasks due dates, they will automatically appear in your daily file when it's time), link other files and start planning your project. The project file contains some automatic queries for:
- **👷‍♀All tasks within project**: Looks for all tasks in files that contain the project tag.
- **🧑‍🤝‍🧑Meetings**: Automatically pulls all meetings that link to the project via the project tag or its file name.
- **↪ Notes & Mentions**: Automatically lists all non-meeting files that link to the project via the project tag or its file name.
## Add files to the project

Project-related notes go in `02_Projects/notes` and canvas files go in `02_Projects/canvas`  if  (see [[Get Started - Obsidian#Canvas|here]] for more info on canvas). 

Create a new note in the `notes/` directory and apply the [[note template]] to it (see [[Create note from template]] for instructions). After the note is created, make sure to first follow the instructions on top of the new note:
- set a link to project file
- set a project name as a tag in the YAML header/properties
Only then, you note will be correctly linked to your template.

Now you can start taking notes. On top of the file, you have tow call-out boxes for convenience: The first one automatically summarizes all tasks in your file and in the second one you can summarize the note content in a few sentences. Feel free to adjust the project not template to your own needs.
## Add a meeting to the project

Meeting notes go in the `03_Meetings/` folder and they follow the naming convention `YYYY-MM-DD meeting name`. To create a meeting, create a new note in the meeting folder, name the note correctly and apply the [[meeting template]]  (see [[Create note from template]] for instructions).
When the note is created, make sure to first follow the instructions on top of the new meeting note:
- set a link to project file below
- set a project name as a tag in the YAML header/properties

In this meeting note you can now plan the meeting but also take notes during the meeting. Also here you have a callout that summarizes all tasks from the meeting note another callout that you can use to summarize the meeting.
The meeting will automatically appear in your project file and in the daily file when it's the date of the meeting.
