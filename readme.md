
# The Exocore Package

![](/images/exocore.png)

## Executive Summary

The exocore is a preconfigured package to roll out your own no-code, no-cost personal website as a public exocortex from documents written in simple Markdown syntax, including interlinking, generated backlinks and a nodal graph-rendering. Site's are rendered in fast, responsive, standards-compliant static HTML. 

The exocore is developed by [Remilia Corporation](https://remilia.org) as a [Jamstack](https://jamstack.org/) worfklow and extension of [Foam](https://github.com/foambubble/foam) to complete the system of an accessible and standardized autopublishing knowledgebase network, as a proof-of-concept for [Remilia's New Internet](https://mirror.xyz/charlemagnefang.eth/831rVsd2Z7cjxnBAw118gW8MylKibfC2AeJ6YUHiAvA).

## Installation Instructions
Follow the [installation-instructions](https://exocore.netlify.app/articles/exocore-installation-instructions/) to install your exocore and set up automatic publishing with Netlify. Time required: ~30 minutes.

## Detailed Introduction

Do you take notes, or conduct personal research? Do you output or collect text or image content in any form, such as a blog, poetry, diary or visual art? Do you intake any form of media, and want to catalogue your findings or thoughts? Do you forget information? The Exocore is a means to store and organize and publish such a bank of information in an easily navigable form.

The exocore comprises a set of a few programs and plugins, rolling them into a package which can be customized infinitely and modularly; without any technical knowledge it can still be made your own, and with even a touch of technical knowledge (particularly CSS or HTML facility) it can be made into anything at all.

Its online component is a scaffolding for a website, and its offline component (fully functional without the online) is a filing system for notes, written output, or other data. Out of the box, it's a local directory of folders and interacting files forming an empty template for a [zettelkasten](https://zettelkasten.de/introduction/)/personal wiki, a platform for longform articles, a library of documents, a gallery of images, and an automatically created daily diary. Mix and match these features as you wish; they are fully modular and independent. A user would be free to use or not use any of these features, so if they want to create a self-hosted platform like Substack with no extra features, this is facilitated.

In the future, these exocores can comprise a webring linked by automatically updated network pages, as well as a IRC network for which the Exocore will operate as user's personal homepages. They can also feature things like an automatically updated 'latest posts' feed from all other (or selected) Exocores, or just 'related posts' (by [metadata](https://jekyllrb.com/docs/front-matter/) tags) from your own site.


# Breaking down the Exocore

![study-monk](/images/study-monk.jpg)

## Information Pipeline

Notes are segregated into 4 categories:
- **Daily Notes**, designed as a quick access scratch pad, and are perfect for low-specificity research dumps and fleeting notes that will inform your notes in future. These are automatically titled by date. One is created each day automatically, and opened when you open VSCode.
- **Wiki Notes**, designed for single atomic data points, and are automatically titled with a hexadecimal color code. This code is turned into a correspondingly colored badge in the index of the published site.
- **Journal Entries**, for your thoughts, and are not automatically titled.
- **Articles**, for longer write-ups on a particular topic.

These note categories together create a pipeline for systematising knowledge over time from the general to the particular, and for capturing a bank of scattered reference material and developing it into a polished final product. For example, you might choose to cite a research dump in the subsequent post that it turned into as a bibliography/further reading section, such as appears at the bottom of [[Predictive Processing and the Free Energy Principle|this wiki note]]. This workflow is designed to encourage active, daily use of the exocore for all thoughts.

## Editing Environment

The exocore is built as an extension on top of the Foam Visual Studio Code package, which is itself an open-source recreation of the Roam learning garden editor. Foam  introduces the standard features required for a proper personal wiki system such as:
- Backlinks panel
- Wikilinks aliasing syntax
- Tiling windows
- Note embedding
- Graph visualization
- Sync files on rename

This system provides a powerful and highly customizable dashboard for comprehensive note-taking. On top of Foam, we've introduced: 
- Segregated note categories with default templates
- Daily note generation
- Automatic randomly generated titling for zettelkasten functionality
- Automatic table of contents generation
- Footnotes and sidenotes
- Suite of Jekyll templates for automatically publishing websites off the collection of notes

### User experience:

A user downloadd the package in the form of a Github repository template, which lives on their local machine as a directory that can be manually or automatically synced via [git](https://git-scm.com) to a web domain, which represents the documents in the directory after they are processed into an eaily-navigable and feature-rich website. Their exocore can be published to the web at no-cost using Netlify's free hosting and subdomain service.

A user can get by just fine only interacting with simple plaintext [markdown](https://www.markdownguide.org) files, and can write posts and create hyperlinks between them, add pictures or PDFs and more, without going beyond in-text markdown syntax (read more about the Exocore's syntax [[Writing with Exocore Syntax|here]]). They are also able to control how their generated website handles their documents in a human-readable [[Using your Exocore#Using Metadata|metadata section]] at the top of each post: tags, title, subtitle, categories, layouts, date, and any others that the user cares to add.

![](/attachments/girl-online.png)

Locally, the directory of notes (which will also be a git repository if you wish to publish as a website online) is managed and maintained through a [VS Code](https://code.visualstudio.com) workspace. 

The recommended extensions for your workspace arrives as a package of two things:

1. A template directory including templates for simple creation of new markdown documents of different kinds (article, journal entry, wiki note, daily note), each treated differently in the rendering of your website.

2. A set of VSCode plugins which offer a suite of features for the user to add to their directory of posts by facilitating easy linking between notes, URL management, and many other features. The directory can be easily hosted for free with [Netlify](https://www.netlify.com), for which a setup guide is available [[Exocore Installation Instructions#Publishing Your Exocore|here]].

### Jekyll

To view your site before it is pushed online, a user can also set up their Exocore directory to build a local instance of the site with [Jekyll](https://jekyllrb.com). When publishing, Netlify runs Jekyll server-side, so running it locally produces the same site as will be published.

### Customizability

The stack is an open-source repo and a suite of open-source programs and plugins, and is therefore ultimately customizable. The level of customizability depends only on your technical know-how, but minimal learnings yield compounding rewards. Here is an idea of the level of control over your final website yielded by advancing levels of technical knowledge:

- **No technical knowledge:**
  - You can implement all of the above, and choose from a set of .CSS templates for your website to adjust its aesthetics. You can create posts, use the daily note functionality, store documents in the Library, create ZK notes and links between them, use backlinking, embed notes, and all other features mentioned above. In other words, all features are fully available with no technical knowledge. You should become acquainted with the Exocore's [[Writing with Exocore Syntax]], but this is easy enough to guess at, or to learn in under half an hour. 

    For publishing, a very cursory knowledge of git will come in handy, but git has a helpful GUI, and Exocore [[Exocore Installation Instructions#Publishing Your Exocore|documentation]] includes a guide on how to publish your site.
  
- **HTML and CSS**
  - You will be able to edit included stylesheets and HTML templates to create a site which looks any way that you wish. Both these languages are simple to learn, and even without learning them comprehensively a user can edit the provided templates and stylesheets to make major changes.  

- **Jekyll/Liquid**
  - You will be able to create logic functions to manipulate metadata stored in the markdown front matter, create custom menus or boxes with automatically generated content based on the front matter, assign your own custom front matter variables, and more. 

- **Ruby**
  - Learning Ruby is not at all necessary, but familiarity with it will facilitate you in packaging themes you have created for your exocore as Ruby Gems in case you would like to publish them for use by others. If you want to proliferate your particular model of the exocore, this is an easy way to package it.


## Full Tech Stack

- [Obsidian](https://obsidian.md) / [VS Code](https://code.visualstudio.com) (and plugin package)
- [Git](https://git-scm.com) (for syncing)
- [Jekyll](https://jekyllrb.com) (for publishing)

**Obsidian Plugins:**
- Backlinks
- Daily Notes
- Templates
- [Obsidian Git](https://github.com/denolehov/obsidian-git)
- [Templater](https://github.com/SilentVoid13/Templater)
- [Filename Heading Sync](https://github.com/dvcrn/obsidian-filename-heading-sync)

**VSCode Plugins:**
- [Foam](https://marketplace.visualstudio.com/items?itemName=foam.foam-vscode)
- [Netlify](https://marketplace.visualstudio.com/items?itemName=shailen.netlify)
- [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)
- [Paste Image](https://marketplace.visualstudio.com/items?itemName=mushan.vscode-paste-image)
- [Spell Right](https://marketplace.visualstudio.com/items?itemName=ban.spellright)

[//begin]: # "Autogenerated link references for markdown compatibility"
[predictive-processing|this wiki note]: _journal/predictive-processing "Predictive Processing and the Free Energy Principle"
[syntax|here]: _articles/syntax "Writing with Exocore Syntax"
[using-exocore#Using Metadata|metadata section]: _articles/using-exocore "Using your Exocore"
[installation-instructions#Publishing Your Exocore|here]: _articles/installation-instructions "Exocore Installation Instructions"
[syntax]: _articles/syntax "Writing with Exocore Syntax"
[installation-instructions#Publishing Your Exocore|documentation]: _articles/installation-instructions "Exocore Installation Instructions"
[//end]: # "Autogenerated link references"
