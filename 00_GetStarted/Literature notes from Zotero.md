# 📚Literature notes from Zotero
*Plugins used:* Templater, Zotero integration

In this vault, you can find an [[schmolkeEcologicalModelsSupporting2010|example of a literature note]] that was created using the [[literature template|vault template for literature notes]]. 

Before you can follow the workflow, you need to setup the connection with Zotero.
## First time Setup
You can find a more detailed walk-through of every step with screenshots [here](https://dannyhatcher.com/zotero-obsidian-integration/).
### Zotero
I assume that you already have [Zotero](https://www.zotero.org/) installed and you know how to use it (add items to your database, attach PDFs to items, read and annotate PDFs).

**Install Better BibTex plugin:**
You need to install the Better BibTex plugin for Zotero. You can find the latest release and a step-by-step installation guide [here](https://retorque.re/zotero-better-bibtex/installation/).
### Zotero integration community plugin
In this demo vault the plugin is already installed and set up to work with the folder structure. If you want to set up everything from the beginning, refer to the step-by-step guide linked above. In any case, you still need to manually download the PDF utility that allows you to extract annotations from the Zotero PDFs. Go to **Settings -> Community Plugins -> Zotero Integration** and download the PDF utility (see screenshot below)

![[Pasted image 20230827200942.png]]
## Create literature notes

Now you are ready to test your workflow. 

> [!warning] Open Zotero
> Make sure that Zotero is running, otherwise you cannot import literature notes and will get an error message

To create a new literature note open the Obsidian command palette (`Ctrl/Cmd + P`) and search for "Zotero Integration: Create Literature Note"

![[Pasted image 20230827201353.png]]

When you hit enter, the Zotero item picker will open and you can pick the item from which to create a literature note. 

> [!tip] What if I don't see the Zotero picker?
>  Sometimes the Zotero picker will not open on top of Obsidian, so you might have to bring the picker to the front from your toolbar.

Just start typing and when you found the right reference, select it and hit enter:

![[Pasted image 20230827201737.png]]

Obsidian will automatically create a literature note in the folder `04_Literature/library` and open the new note. The literature note contains metadata about the paper and a section on annotations that were extracted automatically from the PDF. There is also a section called "Reading notes" where you can add additional notes by hand. See [[schmolkeEcologicalModelsSupporting2010]] for an example of a literature note.

The [[Overview]] file uses Obsidian bases to summarize all your literature notes in one table, so you always know which papers you have already read and taken notes on.
## Update literature notes
To update the literature note with new annotations and content, you just have to create the literature note again, using the steps above. 
Note that this overwrites all the previous content in the literature notes except for the text that is between persistence identifiers like this:

```
%% begin notes %%
%% end notes %%
```

By default, all annotations are persistent. This means that every time you update your note, new annotations are added, but existing ones are not overwritten. The same is true for all the notes in the "Reading notes" section that are between the persistence identifiers.
## More information
- [Official documentation of the plugin](https://github.com/mgmeyers/obsidian-zotero-integration/blob/main/docs/README.md) with hints on how to use it and how to write templates
- [Blogpost with a detailed example workflow](https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
- [Step by step guide](https://dannyhatcher.com/zotero-obsidian-integration/)for the correct setup of Zotero and the plugin with a lot of screenshots and an optional Youtube Video.
- [A long thread on literature note templates](https://forum.obsidian.md/t/zotero-integration-import-templates/36310/235?page=5) where people ask questions and share their templates. This can be a useful reference in case you want to adjust the literature note template. However, all the options might be a bit overwhelming if you are not used to the syntax.
