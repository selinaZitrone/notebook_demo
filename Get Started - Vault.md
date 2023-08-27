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
## Community plugins and functionality

Community plugins are great for extending Obsidian functionality. You can browse, install, remove and configure these plugins from the `Settings` area (gear button on the bottom left). Below, we explain which community plugins we have already preinstalled and what you can do with them.

### Calendar - create daily and weekly notes with one click

Adds the little calendar with the days and the weeks to your notebook. You can click on a specific day or week. Then Obsidian automatically creates a daily/weekly note for the day/week according to your template. The calendar also shows you which day has open tasks (little dot below the day week).

Works well together with: [[Get Started - Vault#Periodic notes|Periodic notes]], [[Get Started - Vault#Templater|Templater]]

### Dataview - Automatically query information in your vault

Treat your Vault as a database which you can query from. Provides a JavaScript API and  
pipeline-based query language for filtering, sorting, and extracting data from Markdown pages. 
It is used within the Daily and Weekly files, e.g. [[2022-W51#🌴 Daily log files of the week]] and the [[Overview]] file of Literature.
Check out the Plugin Website for examples: https://blacksmithgu.github.io/obsidian-dataview/ 

### Emoji shortcodes - Easily add emojis

Insert emojis in your text using the short-codes. E.g. `:purple_heart:` for 💜 or `:see_no_evil:` for 🙈

### Periodic notes
With this plugin you can easily create and navigate between daily and weekly files (also monthly, quarterly or annual files are possible). In the settings of the `Periodic Notes` plugin you can set the templates for your notes and the specific folder, where the new file will be created.  

You can create daily and weekly notes either from the taskbar or from the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar plugin]] by clicking at the respective day or week.

### Tasks
The plugin helps to track tasks within your complete vault. Where ever you format any text like this 
``- [ ] task``
It will be recognised as task. 

Moreover, you can also date the tasks. If you ad a "due to"-date (by clicking in the drop down menu or ... ), the task will appear in the daily log file of the selected day. Here is an example of an open task and a fulfilled task (just click to change the state): 
- [ ] Describe what "tasks" are
- [x] Describe what done tasks are 📅 2022-12-22 ✅ 2022-12-22

Use the Hotkey `Cmd alt t` to edit tasks or search for "Task: Create or edit task" within the command palette. 

Moreover, you can search for tasks within the vault. You can find an example within the daily or weekly files or within the predefined file [[ALL OPEN TASKS]]. 

You can find the documentation of the Plugin here: https://obsidian-tasks-group.github.io/obsidian-tasks/ 

### Templater
The Templater plugin is used to create the templates that are located in the `Templates` folder. In this vault, you can find templates for the daily and weekly files (see [[Get Started - Vault#Periodic notes]]). Of course you can change the templates as best fits your needs.

You can find a full documentation of the Plugin here: https://silentvoid13.github.io/Templater/

# 📖Literature notes from Zotero

In the vault, we use the [Zotero Integration](https://github.com/mgmeyers/obsidian-zotero-integration) community plugin to create literature notes from our Zotero database. What this plugin allows you to do (among other things) is to create a literature note from every item that is in your Zotero library using a custom Obsidian template.

In this vault, you can find an [[SchmolkeEcologicalmodels2010|example of a literature note]] that was created from the [[literature template|vault template for literature notes]].

## Setup

Before you can get started with your own literature notes, there are a couple of things you need to set up in order for the workflow to work as planned. You can find a more detailed walkthrough of every step with screenshots [here](https://dannyhatcher.com/zotero-obsidian-integration/).
### Zotero

I assume that you already have Zotero installed and you know how to use it (add items to your database, attach pdfs to items, read and annotate pdfs).

**Install Better BibTex Add on:**

You need to install the Better BibTex Addon for Zotero. You can find the latest release and a 5-step installation guide [here](https://retorque.re/zotero-better-bibtex/installation/).
### Zotero integration community plugin

In this vault the Zotero-Obsidian integration plugin is already installed and set up to work with the folder structure. If you want to set up everything from the beginning, refer to the step-by-step guide linked above. However, you still need to manually download the PDF utility that allows you to extract annotations from the Zotero PDFs. Go to `Settings -> Community Plugins -> Zotero Integration` and download the PDF utility (see screenshot below)

![[Pasted image 20230827200942.png]]

## Create literature notes

Now you are ready to test your workflow. To create a new literature open the command palette (`Ctrl/Cmd + P`) and look for "Zotero Integration: Create Literature Note"

![[Pasted image 20230827201353.png]]

When you hit enter, the Zotero item picker should open up and Obsidian will wait for you to pick the item you want to create a literature note from. Note that sometimes the Zotero picker will note open on top of your Obsidian, so you might have to check the open Zotero Windows in your toolbar.
Just start typing and when you found the right paper, select it and hit enter:

![[Pasted image 20230827201737.png]]

Now Obsidian will automatically create a literature note for you in the folder `04_Literature/library` and open the file for you. The fill contains all the metadata about the paper and a section on annotations that were extracted from the PDF. The template also contains a "My Notes" section where you can add additional notes by hand.
## More information

- [Blogpost with a detailed example workflow](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
- [Step by step guide](https://dannyhatcher.com/zotero-obsidian-integration/)for the correct setup of Zotero and the plugin with a lot of screenshots and an optional Youtube Video.



