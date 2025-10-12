---
{"dg-publish":true,"permalink":"/digital/digital-garden-plugin/","updated":"2025-10-12T11:47:59.662-07:00"}
---


# Digital Garden by Oleeskild

Official [website](https://dg-docs.ole.dev/) and [Github](https://github.com/oleeskild/obsidian-digital-garden)

An Obsidian plugin that creates a website (or [[Concepts/digital garden\|digital garden]]) from your [[Digital/Obsidian\|Obsidian]] notes. Has many advantages:

- Very few changes needed in your Obsidian files
- Supports many plugins, such as Dataview and Excalidraw!
- Free! (but you should really consider [donating](https://ko-fi.com/oleeskild) )

It has some disadvantages:

- [[Unsorted/WebP\|WebP]] images do not work.
- Note titles are always from the filename. I often want to set my titles in the note, because filenames have character restrictions such as no question marks.
- Tags are a bit weird. Clicking a tag takes you to the search window with the tag prepopulated. I'd prefer a tag page! Thankfully, this is very easy to do myself.  
- The page templates have poor web performance. Their [[Digital/PageSpeed Insights\|PageSpeed Insights]] score is just [37/100](https://pagespeed.web.dev/report?url=https%3A%2F%2Fdg-docs.ole.dev%2Fadvanced%2Fadding-custom-components%2F) as a result of enormous CSS and JS files. I improved performance in the website you're looking at now, but do not expect this if you use the plugin yourself.

## Software engineering details

- Setting up the plugin requires a Github repository to be created in an account you control
- A Github Access token will need to be stored in your vault. If you have any [[Unsorted/Cybersecurity\|Cybersecurity]] experience you should know this token should be treated with great care.
- Publishing or updating a published note causes the plugin to make a new commit in the repository.
- The project uses [Lucide](https://lucide.dev/icons/) icons, which is the same package used by Obsidian.