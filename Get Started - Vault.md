Below, you can find a description of the structure and functionality of this demo vault.
# 📂Folder structure

This vault comes with some suggested folders and workflows. However, every personal workflow is different. Therefore, this is just a suggestion to start with, not a mandatory structure. The predefined folders are:

- **01_Journal**: Folder for Labbook-style files to organize your days/weeks and keep track of tasks and activities.
	- **Daily**: If you create a daily file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
	- **Weekly**: If you create a weekly file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
- **02_Projects**: This is the place for organising and storing project files
	- **canvas**: For Canvas files (for brainstorming etc.)
	- **notes**: For project notes
- **03_Meetings**: Notes for meetings
- **04_Literature**: Here you store and manage your literature notes. 
	- **library:** A subdirectory for your literature notes that you create from your Zotero data base (see [[Get Started - Vault#📖Literature notes from Zotero]] 
	- The `Overview` file automatically creates an overview of all the literature notes in your vault.
- **05_Zettelkasten:** Contains linked notes of your thoughts, ideas and concepts to build your knowledgebase in a Zettelkasten way.
- **Attachments**: All attachments (e.g. PDFs, figures, ...) will automatically be stored here and can be embedded in the notes. 
- **Templates**: In this folder you can find the templates which are used in the different vault workflows

> [!warning] Caution
Please note, that some of the workflows that we set up for this vault depend on the folder names not to change. If you change folder names or names of specific files (especially the templates), some workflows have to be adjusted.

# ⚙Settings and community plugins

We preinstalled and configured some community plugins in this vault that are needed for the [[#🧰Workflows]] described below. 

The following community plugins are installed:
- **Calendar**: Adds a little clickable calendar to your notebook. Used for
	- [[#📆Periodic notes and lab journal]]
- **[Dataview](https://blacksmithgu.github.io/obsidian-dataview/)**:  Provides a JavaScript API and pipeline-based query language for filtering, sorting, and extracting data from Markdown pages. Used for
	- [[#📆Periodic notes and lab journal]]
	- [[#📊 Project management]]
- **Emoji shortcodes**: Insert emojis in your text using the short-codes. E.g. `:purple_heart:` for 💜 or `:see_no_evil:` for 🙈. Used in almost all files to make them look prettier and to mark sections
- **[Periodic notes](https://github.com/liamcain/obsidian-periodic-notes)**: Create and navigate between daily and weekly files (also monthly, quarterly or annual files are possible). Used for
	- [[#📆Periodic notes and lab journal]]
-  **[Tasks](https://obsidian-tasks-group.github.io/obsidian-tasks/)**:  Format, label and track tasks across your entire vault. Can be used in the entire vault but is mainly used in
	- [[#📆Periodic notes and lab journal]]
- **[Templater](https://silentvoid13.github.io/Templater/)**: The Templater plugin is used to create the templates for all workflows.
- **[Zotero integration](https://github.com/mgmeyers/obsidian-zotero-integration)**: With this plugin you can connect your Zotero library with Obsidian and create literature notes, citations and bibliographies. Used in
	- [[#📚Literature notes from Zotero]]

### Periodic notes
With this plugin you can easily create and navigate between daily and weekly files (also monthly, quarterly or annual files are possible). In the settings of the `Periodic Notes` plugin you can set the templates for your notes and the specific folder, where the new file will be created.

You can create daily and weekly notes either from the taskbar (`Ctrl/Cmd + P`) or from the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar plugin]] by clicking at the respective day or week.
### Tasks
The plugin helps to track tasks within your complete vault. Where ever you format text like this 
``- [ ] task``
It will be recognised as task. Moreover, you can also add due dates for your tasks (by clicking the drop down menu that automatically appears).
When a task is done, you can check the checkbox. Here is an example of an open and a closed task:
- [ ] Describe what "tasks" are 📅 2023-08-28 
- [x] Describe what done tasks are 📅 2022-12-22 ✅ 2022-12-22
Use the Hotkey `Cmd alt t` to edit tasks.

You can use a tasks query to automatically load tasks from other files into the current file depending on filters that you can define.
We used this e.g. in the daily and weekly log files to pull tasks with a due date on that day or in that week into the file automatically. E.g. have a look in [[2023-08-23#From the past]] . To see the query you need to click on the `</>` symbol that appears when you hover over the task.
You can find another example of a task query in the file [[ALL OPEN TASKS]]. 

You can find the documentation of the Plugin [here](https://obsidian-tasks-group.github.io/obsidian-tasks/)
### Templater
The Templater plugin is used to create the templates that are located in the `Templates` folder. In this vault, you can find templates for

- Daily and weekly notes ([[daily_template]] and [[weekly_template]])
- Project related notes ([[project template]] for a main project file, [[note_template]] for a note within a project and [[meeting template]] for a project meeting)
- A [[literature template]] for literature notes
- A [[zettel template]] for a note in your Zettelkasten

Of course you can change the templates as best fits your needs.
You can find a full documentation of the plugin [here](https://silentvoid13.github.io/Templater/).
### Zotero integration
With this plugin you can connect your Zotero library with Obsidian and create literature notes using templates. It is used in the workflow for [[#📖Literature notes from Zotero]].
Find the full documentation of the plugin [here](https://github.com/mgmeyers/obsidian-zotero-integration).

# 🧰Workflows
#🚧 This is a very long section... Maybe it makes sense to put every workflow in separate files and only link them here?? Then we might want to create a `Get started` folder inside the vault. But I find this file a bit too long to be convenient to read.... 🚧

Below, you find a description of the most important workflows that we implemented in this vault. Of course you can adapt them as you best fits your needs.
## 📝Create note from template
*Plugins used*: Templater

This workflow is needed for some of the workflows described below. There are different ways to create a template note. The main way that we will use in our workflows is the following:
1. Create a new note in your desired folder (right-click on the folder and say "New Note").
2. Give the note a title (by default it will be named "Untitled")
3. Apply the desired template to the empty note by either #🚧 Maybe these are too many options below? Should we just describe one and if yes which one? 🚧
	1. Hitting the keyboard shortcut `Alt/cmd + E` and selecting the template
	2. Opening the command palette (`Ctrl + P`), search for "Open Insert Template Modal" and select the template you want to insert.
	3. Clicking the Templater button in the left ribbon and then selecting the template you want to insert:
	![[Pasted image 20230828162255.png]]

## 📆Periodic notes and lab journal
*Plugins used*: Calendar, Templater, Periodic Notes, Tasks

The idea of periodic notes is that you use them to track your goals, tasks and work on a daily/weekly basis. In this workflow, we use two templates:
- [[daily_template]]: Create this file every day to get an overview of your tasks and meetings on that day, but also to take notes
- [[weekly_template]]: Create this file every week to plan ahead what you want to focus on and get done in that week. Can also be used to review the week after it's over.
#### Create a periodic note
To create a periodic note for a day/week, first locate the calendar in your notebook (probably either the bottom left corner or in the right side bar). By clicking on a date or week a daily/weekly note is created automatically from the correct template and some information is already filled out. You can find the newly created notes in the folder `01_Journal/Daily|Weekly` . The calendar also shows you which day/week has open tasks (little dot below the day/week).
#### Structure of a daily note (e.g. [[2023-08-23]])
- **Header**: On top, the header automatically contains the date and weekday.
- **🧑‍🤝‍🧑Meetings**: The dataview query in this section automatically looks for meetings that happen on that day. If you want to see the structure of the query, just click on the `</>` symbol in the top right corner of the meeting table. You can use the link in the table to go directly to the meeting file.
- **🐾Tasks**: A section with a task query to automatically find tasks from the past that were forgotten (task due date is over) and tasks that happen today. Here you can also add other tasks for that day manually. When a task is done, just check the checkbox.
- **🏴‍☠Log**: A log section that you can use to log your activities that day, take notes, link other files etc.
- **🗺Changed files**: A list of Obsidian files that you changed that day. This list is automatically compiled with the dataview plugin. Can be useful to easily see the files you worked on that day.
#### Structure of a weekly note (e.g. [[2023-W34]])
- **⛰Goals**: Write down your goals for the week
- **🐾Tasks**: A section that automatically pulls all the tasks for this week into the file. You can manually add other tasks below
- **📜Weekly review**: Space for reviewing the week and planning ahead the next week
## 📊 Project management
*Plugins used*: Templater, Dataview, Tasks

The idea of this workflow is that for every project, you have one main project file in the folder `02_Projects`. This file is your entry point into the project that holds the most important info of your project and links to other notes and meetings relevant for the project.
### Start a new project
To start a new project, create a project file in the `02_Projects` folders and apply the [[project template]] to it (see [[#📝Create note from template]] for instructions). 

>[!warning] Caution 
>In our workflow, we create a corresponding project tag for every project. The tag is called like the project file. Therefore do not use any white space in your project file name. You can e.g. concatenate the file name using underscores

The project file that is created from the template can now be filled with life (see [[project_A|this example file]]). In the project file, you can write down tasks (if you give the tasks due dates, then they will automatically appear in your daily file when it's time), link other files and start planning your project. The project file contains some automatic queries for
- **👷‍♀All tasks within project**: Looks for all tasks that are in files that contain the project specific tag.
- **🧑‍🤝‍🧑Meetings**: Automatically pulls all meetings that link to the project via the project tag
- **↪ Notes & Mentions**: Automatically lists all non-meeting files that link to the project via the project tag.
### Add files to the project
Project-related notes go in the `02_Projects/notes` folder if they are notes, or `02_Projects/canvas` folder if they are canvas files (look [[Get Started - Obsidian#Canvas|here]] for more info on canvas). 
Create a project new note in the `notes/` directory and apply the [[note_template]] to it (see [[#📝Create note from template]] for instructions). When the note is created, make sure to first follow the instructions on top of the new note:
- set a link to project file below
- set a project name as a tag in the YAML header/properties
Only then, you note will be correctly linked to your template.

Now you can start writing down your notes on the bottom of the file. On top, you have tow call-out boxes for convenience: The first one automatically summarizes all tasks that you might have in your file and in the second one you can summarize the note content in a few sentences.

### Add a meeting to the project
Meeting notes go in the `03_Meetings/` folder and they follow the naming convention `YYYY-MM-DD meeting name`. To create a meeting, create a new note in the meeting folder, name the note correctly and apply the [[meeting template]]  (see [[#📝Create note from template]] for instructions).
When the note is created, make sure to first follow the instructions on top of the new meeting note:
- set a link to project file below
- set a project name as a tag in the YAML header/properties

In this meeting note you can now plan the meeting but also take notes during the meeting. Also here you have a callout that summarizes all tasks from the meeting note another callout that you can use to summarize the meeting.
The meeting will automatically appear in your project file and in the daily file when it's the date of the meeting.

## 📚Literature notes from Zotero
*Plugins used:* Templater, Zotero integration

In this vault, you can find an [[SchmolkeEcologicalmodels2010|example of a literature note]] that was created using the [[literature template|vault template for literature notes]]. Before you can follow the workflow, you need to setup the connection with Zotero.
### First time Setup
You can find a more detailed walkthrough of every step with screenshots [here](https://dannyhatcher.com/zotero-obsidian-integration/).
#### Zotero
I assume that you already have Zotero installed and you know how to use it (add items to your database, attach pdfs to items, read and annotate pdfs).

**Install Better BibTex Add on:**
You need to install the Better BibTex Addon for Zotero. You can find the latest release and a 5-step installation guide [here](https://retorque.re/zotero-better-bibtex/installation/).
#### Zotero integration community plugin
In this vault the plugin is already installed and set up to work with the folder structure. If you want to set up everything from the beginning, refer to the step-by-step guide linked above. In any case, you still need to manually download the PDF utility that allows you to extract annotations from the Zotero PDFs. Go to **Settings -> Community Plugins -> Zotero Integration** and download the PDF utility (see screenshot below)

![[Pasted image 20230827200942.png]]
### Create literature notes
Now you are ready to test your workflow. 
> [!tip] Hint
> Make sure that Zotero is also open, otherwise you will get an error mesage

To create a new literature note open the command palette (`Ctrl + P`) and look for "Zotero Integration: Create Literature Note"

![[Pasted image 20230827201353.png]]

When you hit enter, the Zotero item picker should open up and Obsidian will wait for you to pick the item you want to create a literature note from. Note that sometimes the Zotero picker will not open on top of your Obsidian, so you might have to bring the picker to the front from your toolbar.
Just start typing and when you found the right paper, select it and hit enter:

![[Pasted image 20230827201737.png]]

Now Obsidian will automatically create a literature note for you in the folder `04_Literature/library` and open this file for you. The file contains metadata about the paper and a section on annotations that were extracted from the PDF. There is also a section called "My Notes" where you can add additional notes by hand.

The [[Overview]] file uses dataview to summarize your literature notes in a table, so you always know which papers you have already read and taken notes on.
### More information
- [Blogpost with a detailed example workflow](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
- [Step by step guide](https://dannyhatcher.com/zotero-obsidian-integration/)for the correct setup of Zotero and the plugin with a lot of screenshots and an optional Youtube Video.

## 🧠Knowledge management with *Zettelkasten*
*Plugins used:* Templater

The *[Zettelkasten method](https://en.wikipedia.org/wiki/Zettelkasten)* is a tool for personal knowledge management that is based on the idea of small items of information or concepts stored in separate notes that are linked among one another. Obsidian is a perfect tool for implementing such a method to create a sustainable knowledgebase. Here, we describe how to use the basic Zettelkasten system as it is implemented in this vault. Below you can find links that describe the method and different ways of implementing it in Obsidian in more detail.

All single *Zettels* go into the `05_Zettelkasten/` folder. You can already find an example Zettelkasten in this folder. It's probably easiest to understand the method, if you look through the example. You can check out the graph view of this Zettelkasten to see how the notes are connected.
### Add a new Zettel
Just right click on the Zettelkasten folder and say **New note**. The new Zettel is automatically created using the [[zettel template]] and it is opened for you. On top you can give the note a meaningful title.
### Link Zettels
Zettels can and should be linked via 2 concepts: file links and tags.
In every Zettel, you have a callout box on top for "Related topic". Here you can link other Zettels that are related to the current topic. Additionally, you can add tags (either in the front matter or by using the #tag notation) for common topics.
### Add references
Every Zettel has a reference section on the bottom. Here you can put a list of all the references you used to write this Zettel. You can e.g. link a literature note or an external resource.

### More information
- [Youtube video explaining the Zettelkasten method](https://www.youtube.com/watch?v=yqKspwjXu18)
- [Video on Zettelkasten with Obsidian](https://www.youtube.com/watch?v=ziE6UExsOrs)
- [Another video on Zettelkasten with Obsidian](https://www.youtube.com/watch?v=E6ySG7xYgjY)
