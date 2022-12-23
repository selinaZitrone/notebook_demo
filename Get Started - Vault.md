## Folder structure
This vault comes with predefined folders for academic purpose. However, every personal workflow is different. Therefore, we see this as a suggestionto start with, not a mandatory structure. 
The predefined folders are:
- **1_Journal**: Here is the place for regular Labbook-style files
	- **Daily**: If you create a daily file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
	- **Weekly**: If you create a weekly file (for example via the [[Get Started - Vault#Calendar - create daily and weekly notes with one click|Calendar]]) it will be stored here.
- **2_Projects**: This is the place for organising and storing files of your projects
- **3_Literature**: Here you store and manage your literature notes. The `/libary` subdirectory is linked to your Zotero (see [[Get Started - Vault#Citations - create literature notes for papers in your Zotero library|Citations]]) and you can directly import your Zotero annotations. The `Overview` file automatically creates an overview of all the literature notes in your vault.
- **4_Meetings**: Notes for meetings that are created in the Full calendar (see [[Get Started - Vault#Full calendar]]) go here automatically.
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
It is used within the Daily and Weekly files, e.g. [[2022-W51#🌴 Daily log files of the week]] and the [[Overwiew]] file of Literature.
Check out the Plugin Website for examples: https://blacksmithgu.github.io/obsidian-dataview/ 

### Emoji shortcodes - Easily add emojis

Insert emojis in your text using the shortcodes. E.g. `:purple_heart:` for 💜 or `:see_no_evil:` for 🙈

### Full calendar

### Minimal Theme Settings- Control the Appearance of your editor

### Periodic notes
With this plugin you can easily create and navigate between daily and weekly files (also monthly, quaterly or annual files are possible). 
In the settings you can link a plugin and set the specific folder, where the new file will be created. 

### Tasks
The plugin helps to track tasks within your complete vault. Where ever you format any text like this 
``- [ ] task``
It will be recogniced as task. 

Moreover, you can also date the tasks. If you ad a "due to"-date (by clicking in the drop down menu or ... ), the task will appear in the daily log file of the selected day. Here is an example of an open task and a fulfilled task (just click to change the state): 
- [ ] Describe what "tasks" are 📅 2022-12-22 
- [x] Describe what done tasks are 📅 2022-12-22 ✅ 2022-12-22

### Templater
Templater is necessary for the used templates. 


