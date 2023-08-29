Welcome to your Obsidian Notebook. 🎉

This file helps you to get started with Obsidian in general. We explain the basic functionality like markdown syntax, Obsidian settings and functionality. For details on this template vault and its specific workflows, have a look at [[Get Started - Vault]], for further resources on learning cool Obsidian things have  look at [[Get Started - Resources]].

For more information and inspiration on what you can do with Obsidian check out the following tutorial by Nicole van der Hoeven:

#💡 Sollen wir das Video erst später verlinken? Die Leute sollen ja erstmal unsere Sachen lesen und dann in Youtube abdriften

![](https://www.youtube.com/embed/OUrOfIqvGS4)

# 🖥The Obsidian editor

## Navigating Obsidian

In the figure below, you find some important sections of the Obsidian window and what you can do there. But in general: Just experiment and click on the buttons to find out what they do.

![[obsidian_overview.png]]

Please note that you can also change the appearance of Obsidian. It might e.g. be that the calendar in your editor is included in the right sidebar. But you can just drag and drop elements from the sidebar to other locations to change the appearance of the editor.
## Settings

Check out yourself which settings you can change for your Obsidian vault. Just click on the gear icon (⚙) in the bottom left to see what you can do. 
Settings can be changed for general Obsidian things (Appearance, Hotkeys ...) and for the core and community plugins.

## Hotkeys 
You can customize and view all hotkeys in the Obsidian settings. 
Some very essential ones (for my workflow) are: 
- `Ctrl/Cmd + O` : Open quick switcher to open and search for files.
- `Ctrl/Cmd + P` : Open command palette to access commands within Obsidian.
- `Ctrl/Cmd + Shift + F` : Search in all files of Obsidian. 
- `Ctrl/Cmd + Alt + T` : Edit Tasks. 
- `Alt + E` : Select and insert template in note

# ✍ Take notes in Obsidian

## Markdown

Obsidian uses Markdown to format the the text of your notes. 
But as soon as you are finished typing, Obsidian will not show you the markdown syntax anymore but will show you the formatted text. If you click on a formatted element, you will see the markdown version of it. You can try it by clicking on the heading of this section and you will see that there is a `##` in front of the header text.

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

To make text bold or italic, you can also use the keyboard shortcuts you are used to from other programs (Ctrl + B/I on Windows). Have a look at the [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to find more option to format text in Markdown.
## Links

### External resources
Links to external resources work using the markdown syntax for links which is `[Link text](the/actual/link)`. Like this you can for example link to the [Obsidian Website](https://obsidian.md/)
### Internal links
You can link notes within your Obsidian vault by using `[[]]`. For example, I can link to a project note from the project folder like this: [[project_A]].
If you have links to other files in your vault you can
- Click on the link to open the file
- Click while holding `Ctrl/Cmd` to open the file in another tab
- Hover over the link while holding `Ctrl/Cmd` to read the file in a pop up
### Embedded links
Embedded links include the content of the link in your current file. Embedded links work for both external resource links (e.g. to embed Youtube videos) and internal links (e.g. if you want to embed the content of one file into another). All you need to do for this is put an `!` before the link (`![[]]` or `![](https://some/website)`). On top of this file you find an example of an embedded Youtube video.
### Link attachments
You can embed attachments such as images in your notes. You can achieve this by copy/pasting (e.g. a screenshot) or by dragging and dropping a file (e.g. a PNG or a PDF) into your note. These attachments will then be put into your vault and embedded into your note with an embedded link to this resource. Here is an example with a screenshot from the Obsidian website:

![[Pasted image 20230828122500.png]]

You can control where attachments are stored in the Obsidian settings (**Settings -> Files and Links -> Default location for new attachments**)
## Tags
Another way to link files is by using Tags like #tag written as `#tag` .

# 🧩Plugins

There are two types of plugins that you can use to increase the functionality of Obsidian and customize your workflows:

- **Obsidian plugins**: by the Obsidian developers. Can be found under **Settings -> Core plugins**
- **Community plugins**: developed by the community and need to be searched and installed. Can be found under **Settings -> Community plugins**

Be a bit careful with installing community plugins. They run through some basic checks by Obsidian but you install them at your own risk. A good rule of thumb is to install only plugins that are installed by a lot of other users (like 10s of thousands) and that are updated regularly.

#🚧 Should we explain here how to install a community plugin and how to find its settings?
#💡 Ne, das reicht so. 
# 🎁Non-essential but nice to know
## The graph view

The graph view shows you how the files in your vault are linked with each other. For this template vault, the graph looks like this:

![[Pasted image 20221223105640.png]]

You can open the graph view with the Hotkey `Ctrl/Cmd + G` or by clicking on the graph icon in the toolbar on the left. You can also filter your graph by tags or group them. Just explore what you can do.
## Canvas
Canvas is an Obsidian core plugin.

> Canvas allows you to organize notes visually — an infinite space to research, brainstorm, diagram and lay out your ideas.

You can embed your notes alongside images, PDFs, videos, audio, and even fully interactive web pages. 
You find an example in this vault: [[brainstorming.canvas|brainstorming]]
Watch this Youtube video to get more information on how to use the current version of canvas:

![](https://www.youtube.com/embed/G3DJKk4ivq4)

## Callout boxes

The style your files nicely, you can use markdown-style callout boxes that highlight your text. Callout boxes are all written like this: `> [!keyword] title`
Depending on the type of keyword, the boxes look different. You can chose the title however you like. If you leave it blank, a default title will be chosen.
Here you can see examples of all callout boxes you have available:

#🚧 Is this too much examples?
#💡 Haha, so viele gibts da? Ne, ich finde es super die alle mal zu sehen :) 

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


