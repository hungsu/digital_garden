---
{"dg-publish":true,"permalink":"/gear/trim-ui-smart-pro/","updated":"2025-07-02T21:32:45.213-07:00"}
---

![trimui-smart-pro.jpg](/img/user/Embeds/trimui-smart-pro.jpg)
# TrimUI Smart Pro

A teeny tiny [[Unsorted/ARM handheld\|handheld game console]] for nerds, that I bought for $51.52USD including shipping in 2024.

It runs a slimmed down version of Linux, which can run many emulated console games, and a limited number of PC games through an app called [[Digital/Portmaster\|Portmaster]].

It's possible to install a variant of Android on this called [GammaOS](https://github.com/TheGammaSqueeze/GammaOSCore), but I have not tried.

It's a little smaller than [[Gear/Nintendo Switch\|Nintendo Switch]] and a little bigger than my [[Gear/Samsung Galaxy S22\|Samsung Galaxy S22]]. Has Nintendo style button layout on right, which i'm not the biggest fan of as I happen to prefer Xbox and PlayStation style layouts.

Of all the cheap handhelds of 2024, this has the biggest and best screen: 4.96" 1280 × 720p. This is perhaps a bit of a waste since this device is intended to play classic games that have a 4:3 ratio, but I have also enjoyed playing some newer widescreen games on it such as [[Videogames/Dust an Elysian Tale\|Dust: An Elysian Tale]] and [[Videogames/Balatro (2024)\|Balatro (2024)]].

The *Allwinner A133P 1.8GHz CPU* is a bit of a problem. This unusual CPU is so odd that the company Allwinner has not provided 32bit binaries for it. This means many Portmaster games do not work on it.

Has quite meagre specifications:
- 
- 1GB DDR4 RAM. Together these have prevented me from running more demanding emulators and games, such as Hyper Light Drifter and a lot of Nintendo 64 games like Super Smash Bros 64.
- 5000mAh battery, which lasts me around 2 hours

I installed a custom layer over the base operating system, called [Crossmix OS](https://github.com/cizia64/CrossMix-OS), which adds a variety of neat features:
- [[Unsorted/Moonlight\|Moonlight]] for streaming games from [[Gear/my computer\|my computer]], which works well on the device but I've found that the device's weak CPU and RAM seem only able to handle a bitrate of 2.5Mbps. I've observed [one person](https://www.reddit.com/r/trimui/comments/1frgl0u/testing_moonlight_crossmix_os/) say that Moonlight works better at 30FPS on the device, but I'd rather keep the high framerate.
- Function switch remapping - there's a 2-mod switch on the bottom of the device, and its purpose can be defined to do all kinds of things. I set mine to put my console in Turbo mode for more CPU intensive tasks. Note that this seems to make the back of the device quite warm.
- SMB hosting, so when the device connects to WiFi, I can see it as a network drive from my desktop PC. This lets me easily copy game files to it
- Saving state on power off, and booting into saved state on power on

It has one major downside - this OS seems to introduce problems to Portmaster. For example, Death Road To Canada does not work on CrossmixOS, but [allegedly](https://discord.com/channels/1122861252088172575/1122882437291188345/1368701470790123631) does work on Knulli.
## Notes for me and others who own it

The [r/trimui subreddit](https://www.reddit.com/r/trimui/) has made a useful website, [TrimUI Hub](https://destructiveburn.com/TrimUIHub/).

TrimUI have [announced](https://www.reddit.com/r/trimui/comments/1kidhcx/tsp_firmware_v110_and_crossmix_news/) an update to the base OS to v1.1.0, but CrossMix OS does not yet work with this, as of 2025-07-02. The next CrossMix update should somewhat improve Portmaster support.

Some other operating systems exist for the device:
- [Next UI](https://github.com/LoveRetro/NextUI). As of 2025-06-18 it lacks the ability to customise the toggle switch on the bottom of the Smart Pro, so I have not tried this OS yet.
- [Gamma OS](https://github.com/TheGammaSqueeze/GammaOSCore): Notable because it's based on Android TV, opening up the possibility of running Android apps and games on this device.
- [Knulli](https://knulli.org/): Notable to me because [[Digital/Portmaster\|Portmaster]] seems to work better on it. There are some Portmaster games I'm unable to play on CrossMix OS, such as Death Road to Canada.
