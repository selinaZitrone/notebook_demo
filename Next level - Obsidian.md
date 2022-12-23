# Next level - Obsidian
## Zotero citations

The connection between your Zotero database and Obsidian is the `Library.bib` file that is located in the `3_Literature` folder. The idea is to automatically update the `Library.bib` file whenever your Zotero data base changes. This way, Obsidian always has the newest information. 

### Set up Zotero and Obsidian

To set this up, you have to follow these steps:

1. Download and install the `Better BibTeX for Zotero` Add on. Find the installation guide and download link [here](https://retorque.re/zotero-better-bibtex/installation/)
2. Go to `Edit -> Preferences -> Better BibTeX` and change the following settings:
	1. In `Citation keys` create a meaningful citation key format. We have chosen the following that includes authors, short title and year ![[Pasted image 20221223115443.png]]
	2. Configure the `Automatic export` section to export and automatically update a library to your Obsidian vault. Before you do this, go to the vault in your explorer and delete the template `Library.bib` file that we put there. In the `Automatic export section`, configure the export. You can chose if you want to export the whole library, or just a specific folder. Make sure you export the file on change, that the output file is located in your Obsidian vault's literature folder and that you also export the notes you create in Zotero (see pink highlights in screenshot):![[Pasted image 20221223115939.png]]
3. Make sure that Obsidian can find your literature note. Open the settings of the Citations plugin and make sure that `Citation database format` is set to `BibLaTeX`. As citation database path, you need to specifiy the path to your newly created `.bib` file.
4. Try adding a literature note for one of the papers to make sure everything worked correctly (see [[Get Started - Vault#Citations - create literature notes for papers in your Zotero library]] for details).

### Notes and annotations in Zotero

To use this feature at its full potential, you need to know how you can make annotations in Zotero and export them as notes that are then attached to the literature item. This is really easy since Zotero has a PDF viewer integrated. Just do the following:

1. Double click the paper you want to read in Zotero to open it in the Zotero PDF viewer.
2. Read the paper, highlight sections that are important, make little comments
3. Go back to your Zotero database and right click on the paper you just read. Choose `Add Note from Annotations` and you will see that your paper will get an attachment note.
This note will now also be exported in your automatic library in Obsidian. So if you now create a literature note for this item in Obsidian, all your annotations will automatically be included in the `Notes` section of the literature note 🤩.


## Community plugins

### Icon folder
Adds Icons to your folders. 

### Advanced tables 
Helps to work with tables more easily in markdown.

### Activity history
You can track your activity within the vault or specific folders in a Github style.

### Advanced slides
Helps to create slides.

### Banners
Add a graphical banner to each file you want to.

### Natural language dates
More easy use of dates with commands like `@tomorrow` creating automatically next days date. 

### Obsidian git
Do version control from inside Obsidian for your vault.

### Pandoc plugin 
The plugin "adds command palette options to export your notes to a variety of formats including Word Documents, PDFs, ePub books, HTML websites, PowerPoints and LaTeX among (many) others."

### Party 🎉
Confetti as reward if you fulfil a tasks.

### Tag Wrangler
Rename, toggle, merge ... tags in a very easy way! 

### Text generator
"**Text Generator** is an open-source AI Assistant Tool that brings the power of Generative Artificial Intelligence to the power of knowledge creation and organisation in Obsidian.
For example, use Text Generator to generate ideas, attractive titles, summaries, outlines, and whole paragraphs based on your knowledge database."
You need an account for Open AI.

### Tracker
Tracks numbers within your note and helps to visualise them. 


## Markdown
### The YAML header

### Linking and embedding 

Remember, you can link notes within your Obsidian Vault by using `[[]]`. For example, I can link to an example note from the Project folder like this: [[example]]
You can also link to specific headings or section within notes by using a "#" or a "^" like this: [[example#Heading 1.2]] or [[example#^73a7bc]]

By setting an exclamation mark in front of the brackets `![[]]`, , you can embed a file or a subsection of the file. Here is an example: 
![[example#Heading 1.2]]

- [ ] Explain the backlinks and outgoing links section

You can even embed YouTube videos or websites within a note. See a tutorial here: https://patrickberry.medium.com/embed-youtube-video-in-obsidian-efc6f78e35e6




## YouTube Channel about Obsidian
For more information and inspiration on what you can do with Obsidian check out the following YouTube Channels providing insights from basic to advanced use of Obsidian:
- https://www.youtube.com/@nicolevdh
- https://www.youtube.com/@DannyTalksTech 
- https://www.youtube.com/@FromSergio


# Academic note taking 
## Ressources
- https://ilyashabanov.substack.com/p/note-taking-system-for-success-in