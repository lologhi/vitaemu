---
layout: post
title:  "August 09th libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-09 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#5249](https://github.com/libretro/RetroArch/issues/5249) - open - [Vita] glui scrolling - 08/08/2017

When using the glui menu driver navigating through large lists of roms/folders (300+) can cause the selected item to move off the screen, this happens when either scrolling up or down too fast. This has been a problem for a while (since glui was made available to the vita?), and still occurs in both latest stable and nightly releases.

- [#4517](https://github.com/libretro/RetroArch/issues/4517) - open - XMB Horizontal browsing not smooth. - 09/08/2017

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

