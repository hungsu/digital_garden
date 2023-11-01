---
{"dg-publish":true,"permalink":"/software/netlify/"}
---


# ![](https://upload.wikimedia.org/wikipedia/commons/b/b8/Netlify_logo.svg)

[Official site](https://www.netlify.com/)

Host of static websites, and provider of tools such as [NetlifyCMS](https://www.netlifycms.org/),  that simplify and accelerate deployment of those websites.

Nothing to do with Netflix or Shopify.

## Things I like

Netlify bot that automatically makes a test deployment and URL when I make a [[Private/Pull request\|Pull request]] is really handy

## Gotchas

Has bug where all files set to lowercase[^1], thus, you may want to consider alternatives like [[Private/Cloudflare pages\|Cloudflare pages]], [[Software/Github pages\|Github pages]].

> When I started building my startup on Netlify, they moved my personal websites out of their free tier (despite them being in a different account) and into a paid plan. They started charging my card (which I wasn't aware of), and when I changed my billing info they deleted my websites entirely. There was no option to restore them, and their support was incredibly rude. They kept telling me what I had to do to undo their mistake without offering to do it themselves.
One person notes bad behaviours https://news.ycombinator.com/item?id=38062595

[^1]: [Gotcha: Netlify Makes All Your Filenames Case-Insensitive](https://www.jvt.me/posts/2019/11/11/gotcha-netlify-lowercase/) 2019-November-11