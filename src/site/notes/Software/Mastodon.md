---
{"dg-publish":true,"permalink":"/software/mastodon/","title":"Mastodon"}
---


![](/img/user/Vaults/quartz/content/notes/images/mastodon.jpg)

A [[Private/Federated service\|Federated]] social network using [[Private/ActivityPub\|ActivityPub]], competing directly with [[Private/Twitter\|Twitter]] and gaining great interest in 2022-11 with Elon Musk's acquisition of Twitter.

My Mastodon profile is [here](https://mstdn.social/@hungsu), on mstdn.social, one of the larger instances. In the weeks I've been here I've had a few thoughts about Mastodon and federation in general:

## Advantages over Twitter

**No ads or promoted content**. Twitter's ads are *always* repulsive low value content, even when tailored to me. They are either links to blog posts *saturated* with even more ads, or products I never buy.

**No intentional misinformation** (yet). Around 2022-Nov-09, Twitter announced an $8/month subscription it called *verification*. This is a change from Twitter's previous verification method which required government identification. Around 2022-Nov-11, a Twitter account impersonating Eli Lilly tweeted that all insulin would be free. Eli Lilly's stock price tanked afterward.[^1] 

**No algorithm or viral content**. Mastodon has a purely chronological timeline with no algorithm. This means users are left with the thought exercise of finding things of interest.

**No addiction mechanisms or dark patterns**. Since Mastodon has no reason to addict you to it, it can do without Twitter's addictive features, which include:
- Visible likes - On Twitter I found myself skimming over things with few likes and gravitating towards things with many likes. On Mastodon, likes are hidden at first, so you're instead left with just the content to judge on its own merit.
- Quote retweets - Quoting a tweet is a form of performance, speaking to your own audience rather than the person you are quoting. Twitter's history shows that this feature results only in tribal separation rather than discussion. 
- Ratios - Twitter penalised tweets that had too many comments relative to likes, but this meant discussions were discouraged.
- Notifications of people liking replies to you - Twitter looked for any excuse to notify you, and this kind of notification was particularly noisy.

Scott Feeney also has a whole [blog post](https://scott.mn/2022/10/29/twitter_features_mastodon_is_better_without/) on them

**Much nicer people** - on Twitter I frequently encountered people who seemed to be there only to argue and accuse.

## Disadvantages to Twitter

**No one is on there**. None of my friends are there, so I've been forced to have passing interactions with strangers. Fun, but nothing lasting.

**Confusing UX**. Federation is a strange concept to most people. For many, Mastodon is the first federated service they've ever used, myself included. Notably, replying to or following a person on another Mastodon Instance is not straightforward, and requires entering your own username and instance name each time.

## Notable instances

https://social.seattle.wa.us/explore for [[Private/Seattle\|Seattle]] residents
[pkm.social](https://pkm.social/) for [[Concepts/PKM\|PKM]] enthusiasts.

## Helpful tools for getting more out of Mastodon

https://moa.party/ allows automatic posting to twitter from mastodon

If you have your own home page, add this to it to advertise your mastodon 
```HTML
<a rel="me" href="https://your.server/@your_username">Mastodon</a>
```

## Self hosting

If you choose to host Mastodon yourself, be aware that the default settings have scaling problems, such as with a surge of traffic from Twitter exodus:

https://nora.codes/post/scaling-mastodon-in-the-face-of-an-exodus/

[^1]: [Musk’s Twitter chaos tosses outrageous insulin pricing into the spotlight](https://arstechnica.com/science/2022/11/musks-twitter-chaos-tosses-outrageous-insulin-pricing-into-the-spotlight/)