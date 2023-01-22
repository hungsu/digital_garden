---
{"dg-publish":true,"permalink":"/digital-garden-plugin/"}
---


# Digital Garden by Oleeskild

Official [website](https://dg-docs.ole.dev/) and [Github](https://github.com/oleeskild/obsidian-digital-garden)

An Obsidian plugin that creates a website (or Digital Garden) from your Obsidian notes. Has many advantages:

- No additional files needed in your vault
- Very few changes needed in your Obsidian files
- Supports many plugins, such as Dataview and Excalidraw!
- Free! (but you should really consider [donating](https://ko-fi.com/oleeskild) )

It has some disadvantages:

- Note titles are always from the filename. I often want to set my titles in the note, because filenames have character restrictions such as no question marks.
- Tags are a bit weird. Clicking a tag takes you to the search window with the tag prepopulated. I'd prefer a tag page! Thankfully, this is very easy to do myself.  
- No RSS - this is something I might make myself

## Technical details

- Setting up the plugin requires a Github repository to be created in an account you control
- A Github Access token will need to be stored in your vault. If you have any [[Private/Cybersecurity\|Cybersecurity]] experience you should know this token should be treated with great care.
- Publishing or updating a published note causes the plugin to make a new commit in the repository.