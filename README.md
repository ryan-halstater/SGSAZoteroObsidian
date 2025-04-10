# SGSAZoteroObsidian
Supporting documents for 3.25.25 presentation on Zotero and Obsidian

The folder contained is an Obsidian vault with Zotero integration preconfigured for convenience. Instruction for it's construction are below.

Presentation goal: Understand basics of what Zotero and Obsidian have to offer, and have a starting to point to build own notetaking system from if desired.

## Summary
- Zotero: Easy way to store read papers, search, and quickly create bibliographies.
- Obsidian: Notetaking emphasizing links between concepts, easily create searchable and linkable notes on papers from Zotero.
- These are not the only tools! Zotero and Mendeley are competitors for citation management, Obsidian can be replaced by Word or Notion for notetaking and Zotero integration, to name a few. In my opinion, a place to put papers and a place to put synthesis are important to have.

## Zotero: Citation Management Tool
- Adding papers: from browser extension or drag and drop
-   Most metadata fields autopopulate but not always everything -- double check!
- Paper interface: highlights, notes
- Citation Generation
- If interest: organizational tools
  - Tags
  - Searching (basic and advanced)
- Material based on https://www.zotero.org/support/quick_start_guide

## Obsidian: Note-taking tool
- Getting comfortable with vanilla Obsidian
  - Mentioning original philosophy: Zettelkasten/atomicity of thought (some use it as personal wiki, or second brain)
     - Further details https://zettelkasten.de/overview/
  - Download Vault from Github and Open (it is very easy to create own vault too!)
  - Creating and linking notes (latex-compatible!)
  - Quickly: graph view and canvases
  - What the vault looks like from directory view
- Preparing for Zotero integration (based on https://publish.obsidian.md/history-notes/01+Notetaking+for+Historians and https://medium.com/@alexandraphelan/an-updated-academic-workflow-zotero-obsidian-cffef080addd)
  - Install community plugins: Dataview, Zotero Integration
    - Settings > Community plugins > Enable community plugins > browse
    - Dont forget to enable them!
  - Adjusting Zotero Integration options
    - Note Import location: where notes will be added (probably want it to be in Meta folder)
    - Adding Import Path
    - General settings > hotkeys > "import" > add hotkey (makes it much quicker to add paper)
- What can we do?
  - Uploading papers to a template
  - View papers by metadata or links: Dataviews (https://blacksmithgu.github.io/obsidian-dataview/)
    - Written in Database Query Language (DQL) or Javascript
  - Drag and drop in images (will want to change default image location)


# Bonus Resources
- Automatically backing up Obsidian using Github
  - Get git and Github ready
    - ○ Create a local git in folder with Obisidian vault folder, following https://git-scm.com/docs/gittutorial (steps listed below)
  		- § Cd to where Obisidian vault is
  		- § Git init
  		- § Git add .
  		- § Git commit -m "Initial loading"
    - ○ Create private github repo
    - ○ Connect local to github using below steps (sourced from [here]([url](https://docs.github.com/en/migrations/importing-source-code/using-the-command-line-to-import-source-code/adding-locally-hosted-code-to-github#adding-a-local-repository-to-github-using-git)))
      - § Git remote add origin [remote-url from the github, no brackets]
      - § Git remote -v   (to check to see that things worked ok)
      - § Git push origin master
    - ○ Push to remote
  - Getting Obsidian to play nicely
    - ○ Community plugins: git
    - ○ Go back to it, enable, look into options
      - § Can change how often it backs up (My default is every 30 minutes)
  - To backup manually
    - ○ Ctrl p for command palette
    - ○ Run this once on setup to ensure auto-backups will work
      - § Git: commit all chnages
      - § Git: push
- Tool to change citation keys in zotero: https://retorque.re/zotero-better-bibtex/citing/

