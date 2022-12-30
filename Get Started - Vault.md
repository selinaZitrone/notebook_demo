## Folder structure
This vault comes with predefined folders for academic purpose. However, every personal workflow is different. Therefore, we see this as a suggestion to start with, not a mandatory structure. 
The predefined folders are:
- **1_Journal**: Here is the place for regular Labbook-style files
	- **Daily**: If you create a daily file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
	- **Weekly**: If you create a weekly file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
- **2_Projects**: This is the place for organising and storing files of your projects
- **3_Literature**: Here you store and manage your literature notes. The `/libary` subdirectory is linked to your Zotero (see [[Get Started - Vault#Citations - create literature notes for papers in your Zotero library|Citations]]) and you can directly import your Zotero annotations. The `Overview` file automatically creates an overview of all the literature notes in your vault.
- **4_Meetings**: Notes for meetings that are created in the Full calendar (see [[Get Started - Vault#Full calendar]]) go here automatically.
- **Figures**: If you copy and paste figures within any file, the figure will automatically be stored here. 
- **Templates**: In this folder you can find the templates which are used to create the daily and weekly files

## Community plugins and functionality

Community plugins are great for extending Obsidian functionality. You can browse, install, remove and configure these plugins from the `Settings` area (gear button on the bottom left). Below, we explain which community plugins we have already preinstalled and what you can do with them.

### Calendar - create daily and weekly notes with one click

Adds the little calendar with the days and the weeks to your notebook. You can click on a specific day or week. Then Obsidian automatically creates a daily/weekly note for the day/week according to your template. The calendar also shows you which day has open tasks (little dot below the day week).

Works well together with: [[Get Started - Vault#Periodic notes|Periodic notes]], [[Get Started - Vault#Templater|Templater]]

### Citations - create literature notes for papers in your Zotero library

The citations plugin governs how and where your literature notes are created and how you cite literature. The basic idea is the following:

- Have a `.bib` file with all your bibliography inside your vault
- This `.bib` file should automatically update whenever you add new literature and take notes (in Zotero)
- You can search the `.bib` file and create an Obsidian literature not for any of the literature items

We already set this up to work with the template vault and you can have a look at the settings of the citations plugin to see the details and change them. This is the setup and how you can use it:

- There is an example `3_Literature/Library.bib` file in the vault. By default, it is hidden in the Obsidian folder structure, but if you look at your Obsidian vault in your default file explorer, you will see this library file. The library only consists of two papers.
- We already added an example note for you to see how the template for literature notes looks like: [[@aanderudFungalLoopTransfer2018]]. The template is defined in the settings section of the citation plugin and you can adapt it as you like.
- You can add a new literature note by opening the command palette (toolbar on left or hotkey) and searching for the command `Open literature note`. Then you can search for the paper and click on it. The note will then automatically be created in `3_Literature/library` and the filename will be the citation key of the paper. You can now add further notes on the paper and reorder the notes that are already there. 
- You can link to a literature note using `[[]]` as you saw in [[Get Started - Obsidian#Linking Files]] but you can also cite a paper in the text using the citation key with `[]` to get [@aanderudFungalLoopTransfer2018]. You can also achieve this via the command palette and `Insert Markdown citation`.
- The `3_Literature/Overview` file automatically tracks all the literature that you have in your Vault and lists them in a table. This is down using the Dataview plugin (see [[Get Started - Vault#Dataview]] for details).

To see how you can set up your Zotero to work with Obsidian Literature notes, have a look at [[Next level - Obsidian#Zotero citations]].

### Dataview - Automatically query information in your vault

Treat your Vault as a database which you can query from. Provides a JavaScript API and  
pipeline-based query language for filtering, sorting, and extracting data from Markdown pages. 
It is used within the Daily and Weekly files, e.g. [[2022-W51#🌴 Daily log files of the week]] and the [[Overview]] file of Literature.
Check out the Plugin Website for examples: https://blacksmithgu.github.io/obsidian-dataview/ 

### Emoji shortcodes - Easily add emojis

Insert emojis in your text using the short-codes. E.g. `:purple_heart:` for 💜 or `:see_no_evil:` for 🙈

### Full calendar

Full calendar is a useful plugin integrating a calendar feature within Obsidian 📆. You can see the calendar already on the right bottom sidebar (A). But you can also open a full screen version by clicking on the left sidebar (B).

![[Pasted image 20221223165826.png]]

Within the full screen version you can add new calendar entries by clicking and dragging within a day. With every entry a new file is created that you can use to write down your notes concerning the specific event. 

You can find a pretty good documentation about all features and possibilities of the full calendar here: https://davish.github.io/obsidian-full-calendar/ 

### Minimal Theme Settings
Control the Appearance of your editor. You can download community themes under `Settings -> Appearance -> Themes -> Manage`. If you use the `Minimal Theme`, you can control the look of it using the Minimal Theme Settings Plugin. 

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


