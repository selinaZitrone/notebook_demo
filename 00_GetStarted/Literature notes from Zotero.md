# 📚Literature notes from Zotero
*Plugins used:* Templater, Zotero integration

In this vault, you can find an [[SchmolkeEcologicalmodels2010|example of a literature note]] that was created using the [[literature template|vault template for literature notes]]. Before you can follow the workflow, you need to setup the connection with Zotero.
## First time Setup
You can find a more detailed walk-through of every step with screenshots [here](https://dannyhatcher.com/zotero-obsidian-integration/).
### Zotero
I assume that you already have Zotero installed and you know how to use it (add items to your database, attach PDFs to items, read and annotate PDFs).

**Install Better BibTex Add on:**
You need to install the Better BibTex Addon for Zotero. You can find the latest release and a 5-step installation guide [here](https://retorque.re/zotero-better-bibtex/installation/).
### Zotero integration community plugin
In this vault the plugin is already installed and set up to work with the folder structure. If you want to set up everything from the beginning, refer to the step-by-step guide linked above. In any case, you still need to manually download the PDF utility that allows you to extract annotations from the Zotero PDFs. Go to **Settings -> Community Plugins -> Zotero Integration** and download the PDF utility (see screenshot below)

![[Pasted image 20230827200942.png]]
## Create literature notes
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
## More information
- [Blogpost with a detailed example workflow](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
- [Step by step guide](https://dannyhatcher.com/zotero-obsidian-integration/)for the correct setup of Zotero and the plugin with a lot of screenshots and an optional Youtube Video.

