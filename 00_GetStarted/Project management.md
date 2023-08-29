# 📊 Project management
*Plugins used*: Templater, Dataview, Tasks

The idea of this workflow is that for every project, you have one main project file in the folder `02_Projects`. This file is your entry point into the project that holds the most important info of your project and links to other notes and meetings relevant for the project.
## Start a new project
To start a new project, create a project file in the `02_Projects` folders and apply the [[project template]] to it (see [[Create note from template]] for instructions). 

>[!warning] Caution 
>In our workflow, we create a corresponding project tag for every project. The tag is called like the project file. Therefore do not use any white space in your project file name. You can e.g. concatenate the file name using underscores.

The project file that is created from the template can now be filled with life (see [[project_A|this example file]]). In the project file, you can write down tasks (if you give the tasks due dates, then they will automatically appear in your daily file when it's time), link other files and start planning your project. The project file contains some automatic queries for:
- **👷‍♀All tasks within project**: Looks for all tasks that are in files that contain the project specific tag.
- **🧑‍🤝‍🧑Meetings**: Automatically pulls all meetings that link to the project via the project tag.
- **↪ Notes & Mentions**: Automatically lists all non-meeting files that link to the project via the project tag.
## Add files to the project
Project-related notes go in the `02_Projects/notes` folder if they are notes, or `02_Projects/canvas` folder if they are canvas files (look [[Get Started - Obsidian#Canvas|here]] for more info on canvas). 
Create a new note in the `notes/` directory and apply the [[note_template]] to it (see [[#📝Create note from template]] for instructions). When the note is created, make sure to first follow the instructions on top of the new note:
- set a link to project file below
- set a project name as a tag in the YAML header/properties
Only then, you note will be correctly linked to your template.

Now you can start writing down your notes on the bottom of the file. On top, you have tow call-out boxes for convenience: The first one automatically summarizes all tasks that you might have in your file and in the second one you can summarize the note content in a few sentences.

## Add a meeting to the project
Meeting notes go in the `03_Meetings/` folder and they follow the naming convention `YYYY-MM-DD meeting name`. To create a meeting, create a new note in the meeting folder, name the note correctly and apply the [[meeting template]]  (see [[#📝Create note from template]] for instructions).
When the note is created, make sure to first follow the instructions on top of the new meeting note:
- set a link to project file below
- set a project name as a tag in the YAML header/properties

In this meeting note you can now plan the meeting but also take notes during the meeting. Also here you have a callout that summarizes all tasks from the meeting note another callout that you can use to summarize the meeting.
The meeting will automatically appear in your project file and in the daily file when it's the date of the meeting.
