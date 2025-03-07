---
{"dg-publish":true,"permalink":"/obsidian-livesync/"}
---


> [!info] Caveat
> I am a software engineer by profession, and to use LiveSync you will likely need to be in a similar trade or at least be very computer savvy. I have never used Obsidian’s official paid Sync.

LiveSync is an [[Private/Obsidian plugin\|Obsidian plugin]] which I am using to synchronise my Obsidian vault between my Android phone and two Windows computers. It replaced [[Digital/Resilio Sync\|Resilio Sync]] and [[Private/Syncthing\|Syncthing]] for me.

Resilio and Syncthing worked for years, but with significant issues:

- Conflicts and conflict resolution. Syncthing had a tendency to imagine conflicts when there was no reason to think so. Something as simple as adding content to a file might cause Syncthing to complain and ask me to manually resolve a conflict, which would just be me accepting the additional content I wrote. Other times, the conflicts would be complex, and I would be forced to use a text editor to resolve conflicts like I was writing code. This costs me lots of time and takes me well out of writing flow
- Resilio Sync has had somewhat the opposite problem. I could change a file in two places, and instead of telling me to merge things together, Resilio would simply overwrite the file with the oldest date with the file with the newest date, even if the old file has more content. I have lost significant content this way.

Since 2025-01 I’ve switched over to [Obsidian LiveSync](https://github.com/vrtmrz/obsidian-livesync). It has worked almost flawlessly to keep Obsidian synced on my 3 devices.

I have not had to resolve a conflict even once. I have lost content just once - I opened my daily note on my phone when I had already created on on my desktop, before the desktop's version could be copied over.

Since moving to LiveSync, I can simply write and think about writing instead of thinking about syncing.

Obsidian LiveSync itself is free. It requires MongoDB set up somewhere such as Fly.io. Fly.io requires a credit card and may cost money. For small vaults under 1GB and small usage this should be free. Vaults that are over 1GB or sync many megabytes a day would probably incur a cost.

It was somewhat tricky to set up. I considered following the more manual instructions, but ultimately chose the [quick start method](https://github.com/vrtmrz/obsidian-livesync/blob/main/docs/setup_flyio.md#a-very-automated-setup) in the readme using Fly.io. Again, I’m a software engineer and if this document looks scary then this is probably not the approach for you.

My vault is around 12000 files, and LiveSync’s initial setup took a long time. I foolishly did this on a laptop that kept going to sleep during the process, and in retrospect I should have started this on my desktop PC, or started with a fresh empty vault and gradually moved files into it instead.  
  
If any of you have been frustrated trying to synchronise Obsidian between multiple devices, this may be an option for you
