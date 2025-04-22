---
{"dg-publish":true,"permalink":"/digital/hugo/"}
---

# Hugo

A [[Private/Static site generator\|Static site generator]] built in [[Private/Golang\|Golang]]. Has a reputation for being incredibly fast, and feature rich.

It also has a reputation for having terrible documentation. So terrible that it drives users to alternatives, such as NextJS or [Zola](https://www.getzola.org/).
- [Hugo is great, it's documentation is not](https://sagar.se/blog/hugo-documentation/)
 - this article is also a great write up of [[Private/Technical writing\|Technical writing]] and [[Public/Atomic notes\|Atomic notes]]
 - There is a user made quick start guide here: [Minimum Viable Hugo](https://github.com/hiAndrewQuinn/minimum-viable-hugo)

Fireship did a video about [Hugo in 100 seconds](https://www.youtube.com/watch?v=0RKpf3rK57I)

## Testimonials

### Happy
> When building a large website (kde.org has more than 1400 pages) all these features make sense. I can organize my template in directories, enjoy fast generation time, separating the templating part from the content, create SCSS files for each pages that needs a special layout. There is also a (fast) JS bundler integrated into Hugo. Afaik Zola also doesn't support i18n and Jekyll has a few plugins for that but this is not a build-in functionality.
> — [2020-10-30](https://news.ycombinator.com/item?id=24945745)

> Build times went from 10 seconds to 0.2s.
> — [seanwilson](https://news.ycombinator.com/item?id=24946414)

> it has enough built in (Sass, minifying, JavaScript bundler, image optimisation) that you just focus on site content rather than procrastinating with your build chain.
> — [seanwilson](https://news.ycombinator.com/item?id=24946414)

### Not so happy
> My most frustrating experience with Hugo is their template language and lack of clear explanations, often waiving away any complexities as, “They’re just Go templates.” Fair enough, but the docs make no attempt to explain how scoping works, how variables can be applied to partials, or even how to construct a simple for-loop. There’s an answer for each of these problems but implementing a full solution requires scouring through the Go docs and Hugo’s own forums for a complete and pragmatic solution.
> —[A throwaway account](https://news.ycombinator.com/item?id=30528827)

> But much like Handlebars, Go template expressions aren’t REPL friendly, and a the learning experience involves a lot of refreshing and debug output just to get a clue as to how things work.
> —[A throwaway account](https://news.ycombinator.com/item?id=30528827)

> The whole "They Are Just Go Templates" is a pretty pathetic cop out. Sorry, but it's true. If I'm trying to use Hugo, I don't want to be digging in Go docs at the same time, and as you point out, you can't know things like scopes and what Go variables might actually be available...I subsequently gave up on Hugo entirely and ported my Hugo sites to Next.js, which is in fact documented--and can work well with TypeScript, so complex pages are fully strongly typed, which makes work in an IDE a breeze. 
> —[SomeCallMeTim](https://news.ycombinator.com/item?id=30533110)