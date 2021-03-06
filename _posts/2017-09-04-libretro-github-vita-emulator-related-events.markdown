---
layout: post
title:  "September 04th libretro updates concerning PS Vita emulation and emulators"
date:   2017-09-04 06:00:02 +0200
categories: vita emulation
---

### RetroArch
- [#4517](https://github.com/libretro/RetroArch/issues/4517) - open - XMB Horizontal browsing not smooth. - 03/09/2017

When you have multiple playlists and some of them are huge, XMB will halt on them.

Keeping the right direction pushed down will stop the browsing for a while on my big Mame playlist (5s).
To speed it up a bit I have to release the direction, and try to push again several times until it moves.
If I don't the browsing will get really slow at proceeding through every item (1s-2s each).

That's an extreme case playlist of 75000+ lines but 10000 lines (complete romset of many systems) is enough to make strong hiccups.

Would it be possible to limit the entries loaded when simply browsing left-right to optimize this?

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/41393572-xmb-horizontal-browsing-not-smooth?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

### vba-next
- [#76](https://github.com/libretro/vba-next/issues/76) - open - (Vita) Wario Ware Twisted (U) - Crash during Dribble & Spitz end cutscene - 03/09/2017

This crash occurs with the latest nightly, it happens when the space taxi cab go offscreen. Since the cutscene is unskippable, I can't progress in the game anymore.
There's another crash in this game with a Mona mini-game but I'm unable to tell which one because it crashes before it appears.

This contains the crash dump generated by the Vita and the savestate before the crash: 
[vita_wwt_crash.zip](https://github.com/libretro/vba-next/files/601705/vita_wwt_crash.zip)

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/39385830-vita-wario-ware-twisted-u-crash-during-dribble-spitz-end-cutscene?utm_campaign=plugin&utm_content=tracker%2F1027743&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F1027743&utm_medium=issues&utm_source=github).
</bountysource-plugin>

