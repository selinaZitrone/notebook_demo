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


### Calendar - create daily and weekly notes with one click
Adds the little calendar with the days and the weeks to your notebook. You can find the calendar in the bottom left corner or in the right side bar of the Obsidian editor. Clicking on a date or week automatically creates a daily/weekly note for that day/week using the respective template from the template. The calendar also shows you which day has open tasks (little dot below the day week).

Works well together with: [[Get Started - Vault#Periodic notes|Periodic notes]], [[Get Started - Vault#Templater|Templater]]
### Dataview - Automatically query information in your vault
Provides a JavaScript API and pipeline-based query language for filtering, sorting, and extracting data from Markdown pages. 
It is used within the Daily and Weekly files, e.g. [[2023-W34#🌴 Daily log files of the week]] and the [[Overview]] file of literature notes.

Check out the [Dataview website](https://blacksmithgu.github.io/obsidian-dataview/) for examples.

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

Below, you find a description of the most important workflows that we implemented in this vault. Of course you can adapt them as you best fits your needs.
## 📝Create note from template
This workflow is needed for some of the workflows described below. There are different ways to create a template note. The main way that we will use in our workflows is the following:
1. Create a new note in your desired folder (right-click on the folder and say "New Note").
2. Give the note a title (by default it will be named "Untitled")
3. Apply the desired template to the empty note by either #🚧 Maybe these are too many options below? Should we just describe one and if yes which one? 🚧
	1. Hitting the keyboard shortcut `Alt/cmd + E` and selecting the template
	2. Opening the command palette (`Ctrl + P`), search for "Open Insert Template Modal" and select the template you want to insert.
	3. Clicking the Templater button in the left ribbon and then selecting the template you want to insert:
	![[Pasted image 20230828162255.png]]

## 📆Periodic notes and lab journal

## 📊 Project management

## 📚Literature notes from Zotero

In the vault, we use the [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration) community plugin to create literature notes from our Zotero database. What this plugin allows you to do (among other things) is to create a literature note from every item that is in your Zotero library using a custom Obsidian template.

In this vault, you can find an [[SchmolkeEcologicalmodels2010|example of a literature note]] that was created using the [[literature template|vault template for literature notes]].
### First time Setup
Before you can get started with your own literature notes, there are a couple of things you need to set up in order for the workflow to work as planned. You can find a more detailed walkthrough of every step with screenshots [here](https://dannyhatcher.com/zotero-obsidian-integration/).
#### Zotero
I assume that you already have Zotero installed and you know how to use it (add items to your database, attach pdfs to items, read and annotate pdfs).

**Install Better BibTex Add on:**
You need to install the Better BibTex Addon for Zotero. You can find the latest release and a 5-step installation guide [here](https://retorque.re/zotero-better-bibtex/installation/).
#### Zotero integration community plugin
In this vault the Zotero-Obsidian integration plugin is already installed and set up to work with the folder structure. If you want to set up everything from the beginning, refer to the step-by-step guide linked above. However, you still need to manually download the PDF utility that allows you to extract annotations from the Zotero PDFs. Go to `Settings -> Community Plugins -> Zotero Integration` and download the PDF utility (see screenshot below)

![[Pasted image 20230827200942.png]]
### Create literature notes
Now you are ready to test your workflow. 
> [!tip] Hint
> Make sure that Zotero is also running, otherwise you will get an error mesage

To create a new literature open the command palette (`Ctrl/Cmd + P`) and look for "Zotero Integration: Create Literature Note"

![[Pasted image 20230827201353.png]]

When you hit enter, the Zotero item picker should open up and Obsidian will wait for you to pick the item you want to create a literature note from. Note that sometimes the Zotero picker will note open on top of your Obsidian, so you might have to check the open Zotero Windows in your toolbar.
Just start typing and when you found the right paper, select it and hit enter:

![[Pasted image 20230827201737.png]]

Now Obsidian will automatically create a literature note for you in the folder `04_Literature/library` and open the file for you. The fill contains all the metadata about the paper and a section on annotations that were extracted from the PDF. The template also contains a "My Notes" section where you can add additional notes by hand.
### More information
- [Blogpost with a detailed example workflow](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
- [Step by step guide](https://dannyhatcher.com/zotero-obsidian-integration/)for the correct setup of Zotero and the plugin with a lot of screenshots and an optional Youtube Video.

## 🧠Knowledge management with Zettelkasten

