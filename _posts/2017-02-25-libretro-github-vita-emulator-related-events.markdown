---
layout: post
title:  "February 25th libretro updates concerning PS Vita emulation and emulators"
date:   2017-02-25 06:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#4517](https://github.com/libretro/RetroArch/issues/4517) - open - XMB Horizontal browsing not smooth. - 24/02/2017

When you have multiple playlists and some of them are huge, XMB will halt on them.

Keeping the right direction pushed down will stop the browsing for a while on my big Mame playlist (5s).
To speed it up a bit I have to release the direction, and try to push again several times until it moves.
If I don't the browsing will get really slow at proceeding through every item (1s-2s each).

That's an extreme case playlist of 75000+ lines but 10000 lines (complete romset of many systems) is enough to make strong hiccups.

Would it be possible to limit the entries loaded when simply browsing left-right to optimize this?

