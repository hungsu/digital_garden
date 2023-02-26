---
{"dg-publish":true,"permalink":"/software/quartz-by-jacky/","title":"Quartz"}
---


# Quartz

A tool for publishing [[Software/Obsidian\|Obsidian]] to the web as a [[Concepts/digital garden\|digital garden]], and what I once used to publish what you are reading now.

It's built on top of [[Software/Hugo\|Hugo]] which I'm told is very fast, but can be hard to use. So far I've observed builds with this tool taking around 40 seconds which is a bit slower than I'd like. My previous tool used Jekyll and took around 20 seconds.

The [Official Quartz website](http://quartz.jzhao.xyz/) has the instructions I followed to make this.

## Why I stopped using it

**Weird formatting requirements**. Obsidian allows you to refer to a note without mentioning its path, such as `[[software engineering]]`. Quartz requires you to use Markdown links `[]()`, with a full path and URL encoding of spaces. Attempting to use wikilinks anyway will result in broken links and backlinks. This has another consequence, Obsidian is unable to automatically update links in this format if you rename or move them.

Overall this made publishing more difficult, and maintenance of my vault difficult.

**Missing features**. For example, inline tags, like `#claim`  will just appear as plain text. I requested support for these in [this ticket](https://github.com/jackyzha0/quartz/issues/161).

## Other drawbacks

- Significant technical knowledge needed. I had to install [[Private/Golang\|Golang]], Hugo, Make, add those to my environment path, just to build the website on my Windows laptop. For the tech savvy it doesn't feel like much, but this is too difficult for many people. 
- No RSS. Jacky has teased the idea of possibly adding it in future, on the Quartz Discord.
- Poor [[Private/Accessibility\|Accessibility]] for screen readers. This comes in a few forms:
	- The search button is not a button. This is fixed in these notes, but still a problem in the original source.
	- No alt text on images. Markdown supports adding some text to an image like so: `![Some alt text](link\to\image.jpg)`. But either Quartz or Hugo ignores it.

## Why I liked Quartz

All the words above may seem like I dislike Quartz. I enjoyed my time with Quartz, it just so happens I found something better!

- **Separate note titles, filenames, and link text**. One of the solutions I tried previously, Foam Research, required that note titles, filenames, and link text all be the same, and in a particular format. For instance, a Quartz link can look like `any text that I want even emoji`, but a Foam link always looks like:  `hyphens-and-lower-case`, including the dashes. This was maddening!
- **Interactive graph**. Quartz has a much more friendly graph than others I've tried so far, with nice hover effects, bouncy physics, and even links between neighbours!
- **Dark mode**. I often read my own notes at night, and appreciate being able to set the theme to dark mode.
- **Backlinks with context**. A list of backlinks would appear at the bottom of a page. If you hovered over the backlink, you would see the sentence that refers to the current page. This is amazing! [[Claims/Backlinks should include context\|Backlinks should include context]]!

## Alternatives I didn't like, but you might

- [[Software/Obsidian Publish\|Obsidian Publish]], but people seem to have mixed things to say about it.
- [Jekyll](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll). These notes you're reading used to be published this way. There are other ways to use Jekyll, but the method I linked seems to be the most comprehensive.
