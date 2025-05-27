---
{"dg-publish":true,"permalink":"/unsorted/drop-cap/","updated":"2025-05-12T01:53:25.452-07:00"}
---


# Drop cap

![](https://www.si.edu/sites/default/files/styles/grid_large/public/acm-acmobj-201100040106.jpg?itok=64742OMT&c=73a396a07e902f262268ccedb98e7822)

A piece of [[Unsorted/typography\|typographic flair]]  added to the first letter of an important paragraph, often the first paragraph of an entire piece of writing (though not always).

## Pretty examples

[[People/Gwern Branwen\|Gwern Branwen]] has pretty drop caps on his [website](https://www.gwern.net/LARPing), but only on large screens.

![gwern_drop_cap.png](/img/user/Embeds/gwern_drop_cap.png)

Well and Good have a lot of padding around their drop caps
![Drop cap - Well and Good.jpg](/img/user/Embeds/Drop%20cap%20-%20Well%20and%20Good.jpg)

[[Unsorted/The MIT Press Reader\|The MIT Press Reader]] colours their drop cap the same colour as its logo:
![firefox_VmKW61PDi8.jpg](/img/user/Embeds/firefox_VmKW61PDi8.jpg)

[[Unsorted/The Atlantic\|The Atlantic]] uses a separate font, *Atlantic Serif* for its drop cap, and yet another font in small caps for the first stretch of words, *Adobe Garamond Pro*.

![TheAtlantic_dropcap.jpg](/img/user/Embeds/TheAtlantic_dropcap.jpg)

https://www.eviemagazine.com/post/elon-musk-permanently-bans-twitter-account-pedophilia-pride-flag-youth-attracted 

## Working with drop caps

Drop caps for web are generally implemented with the CSS pseudoclass, `::first-letter` . Any browser dev tools should work for analysing drop caps on the web. Firefox's dev tools has them under the pseudo elements section.

It should also be noted that using `:first-letter` is best for accessibility. Other methods using an element wrapping the first letter cause problems with [[Unsorted/screen reader\|screen reader]]s.[^1]

![Drop cap](https://blog.stephaniestimac.com/img/2023/initial-letter/initial-letter.png)

Some browsers have introduced the `initial-letter` [[Unsorted/CSS\|CSS]] property, which gives a reliable way to set the height of a drop cap. This allows large illustrated drop caps like above.


This is supported on Safari, Edge, and Chrome.[^3]

[^1]: [Smashing Magazine](https://www.smashingmagazine.com/2012/04/drop-caps-historical-use-and-current-best-practices/) Historical Use And Current Best Practices With CSS , 2012 April 4

https://blog.stephaniestimac.com/posts/2023/1/css-initial-letter/

[^3]: [Can I use](https://caniuse.com/?search=initial-letter) initial-letter