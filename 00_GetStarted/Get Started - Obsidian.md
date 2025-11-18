# Get Started - Obsidian
Welcome to your Obsidian Notebook. 🎉

This file helps you to get started with Obsidian in general. We explain the basic functionality like markdown syntax, settings and functionality. For details on this demo vault and its specific workflows, have a look at [[Get Started - Vault]], for further resources on Obsidian check out [[Get Started - Resources]].

## 🖥The Obsidian editor

### Navigating Obsidian

In the figure below, I highlighted the important areas of the Obsidian workspace and what you can do there. Your layout might look sightly different (e.g. the Calendar might be in the top right sidebar for you). But in general: Just have a look at all the buttons, experiment and click on them to find out what they do.


![[obsidian_overview.png]]


> [!tip] Customize your layout
> You can customize the Obsidian layout by dragging and dropping elements. You can for example drag the Calendar to the right side bar or even grab the entire file navigation on move it around. 
### Settings

You can find the Obsidian settings by clicking on the gear icon (⚙) in the bottom left. Just have a look around to see what you can do there. Settings can be changed for general Obsidian things (Appearance, Hotkeys ...) and for the core and community plugins.

### Hotkeys 
You can customize and view all hotkeys in the Obsidian settings. 
Some very essential ones (for our workflow) are: 
- `Ctrl/Cmd + O` : Open quick switcher to open and search for files.
- `Ctrl/Cmd + P` : Open command palette to access commands within Obsidian.
- `Ctrl/Cmd + Shift + F` : Search in all files of Obsidian. 
- `Ctrl/Cmd + Alt/Option + T` : Edit Tasks. 
- `Alt/Option + E` : Select and insert template in note

## ✍ Take notes in Obsidian

### Markdown

Obsidian uses Markdown to format the the text of your notes. 
As soon as you are finished typing, Obsidian will not show you the markdown syntax anymore but will show you the formatted text. If you click on a formatted element, you will see the markdown version of it. You can try it by clicking on the heading of this section and you will see that there is a `##` in front of the header text.

This is the most basic Markdown syntax:

```md
# Heading 1
## Heading 2
### Heading 3
#### Heading 4

**bold**
*italic*

[A Link](https://google.com)

- list
- list
- list

1. numbered list
2. numbered list

- [ ] A task
- [x] A fulfilled task
```

To make text bold or italic, you can also use the keyboard shortcuts you are used to from other programs (`Ctrl/Cmd + B/I`). Have a look at the [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) for a more comprehensive list of Markdown formatting.
### Links

#### External resources
Link to external resources work with the markdown syntax for links which is `[Link text](https://the/actual/link)`. You can also use the keyboard shortcut `Ctrl/Cmd + K` to insert the link skeleton. Links to external resources then look like this: [Obsidian Website](https://obsidian.md/)
#### Internal links
You can link notes within your Obsidian vault by using `[[]]`. For example, I can link to a note from the project folder like this: [[project_A]].
If you have links to other files in your vault you can
- Click on the link to open the file
- Click while holding `Ctrl/Cmd` to open the file in another tab
- Hover over the link while holding `Ctrl/Cmd` to read the file in a pop up
#### Embedded links
Embedded links include the content of the link in your current file. Embedded links work for both external resource links (e.g. to embed Youtube videos) and internal links (e.g. if you want to embed the content of one file into another). All you need to do for this is put an `!` before the link (`![[]]` or `![](https://some/website)`). You can have a look at [[Get Started - Obsidian]] where we embedded a YouTube Video using this system.
#### Link attachments
You can embed attachments such as images in your notes. You can achieve this by copy/pasting (e.g. a screenshot) or by dragging and dropping a file (e.g. a PNG or a PDF) into your note. The attachment (i.e. the PDF/PNG) will be added to your vault and embedded into your note with an embedded link to the file. Here is an example with a screenshot from the Obsidian website:

![[Pasted image 20230828122500.png]]


> [!tip] Control attachment locations
> You can control where attachments are stored in the Obsidian settings (**Settings -> Files and Links -> Default location for new attachments**)
### Tags
You can use tags to group and link files. Just put he `#` symbol before a word (without space in between) `#tag` becomes a #tag. You also search files by tag in the search bar.

## 🧩Plugins

There are two types of plugins that you can use to customize the functionality and workflows of Obsidian:

- **Obsidian plugins**: by the Obsidian developers. Can be found under **Settings -> Core plugins**
- **Community plugins**: developed by the community; need to be searched and installed. Can be found under **Settings -> Community plugins**

Be a bit careful with installing community plugins. They run through some basic checks by Obsidian but you install them at your own risk. A good rule of thumb is to install only plugins that are installed by a lot of other users (like 10s of thousands) and that are updated regularly.

To check which community plugins are installed in this demo vault, have a look at [[Get Started - Vault#⚙Settings and community plugins]]. To check out which additional cool community plugins we recommend to check out, have a look at [[Get Started - Resources#🧩 Community plugins]]
## 🎁Non-essential but nice to know
### The graph view

The graph view visualizes how the files are linked in your vault. For this template vault, the full graph looks like this:
![[Pasted image 20230829165829.png]]
You can open the graph view with the Hotkey `Ctrl/Cmd + G` or by clicking on the graph icon in the toolbar on the left. You can also filter your graph by tags or group them. Just explore what you can do.
### Canvas
Canvas is an Obsidian core plugin which allows you to organize notes visually. It can be used to brainstorm, create mindmaps, flowcharts and more.
You can embed your notes alongside images, PDFs, videos, audio, and even fully interactive web pages. You find an example in this vault (it is an embedded link, so just click on the flowchart and the file will open): 

![[brainstorming.canvas|brainstorming]]


To create a new Canvas, just open the Command palette (`Ctrl/Cmd + P`) and search for "Create new Canvas". You can just experiment a bit what you can do there. You can also watch this youtube video to get an idea of how you can use Canvas:

![](https://www.youtube.com/watch?v=HFK3D7zeyTA)

### Callout boxes

You can style and highlight your text by using callout boxes. Callout boxes are written like this:

```
> [!keyword] Box with title only
```

> [!keyword] Box with title only

``` 
> [!keyword] Box with title and content
> Some Content of the box
```

> [!keyword] Box with title and content
> Some Content of the box

``` 
> [!keyword]- Click on the arrow to unfold content
> Some Content of the box that can be unfolded
```

> [!keyword]- Click on the arrow to unfold content
> Some Content of the box that can be unfolded

Depending on the type of keyword, the boxes look different. 
Here you can see examples of all callout boxes you have available:

> [!Note]

> [!abstract] abstract / summary / tldr

> [!info] info / todo

> [!tip] tip / hint / important

> [!done] success / check / done

> [!faq] question / help / faq

> [!warning] warning / caution / attention

> [!failure] failure / fail / missing

> [!danger] danger / error

> [!bug] bug

> [!example] example

> [!quote] quote


