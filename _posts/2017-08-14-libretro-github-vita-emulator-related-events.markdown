---
layout: post
title:  "August 14th libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-14 06:00:02 +0200
categories: vita emulation
---

### RetroArch
- [#5293](https://github.com/libretro/RetroArch/issues/5293) - open - 1.6.4 PS Vita - Online Updater - Thumbnails Updater fails - 13/08/2017


## Description
Using Retroarch 1.6.4 for PS Vita, Thumbnails Updater fails. 

### Expected behavior

Thumbnails Updater should download and extract selected thumbnails to directory 

### Actual behavior

Thumbnails download will get to about 50%, than restart itself - showing text indicating 0% before finally failing with 'Task Failed'.


Tested with Mega Drive, Nintendo - Nintendo Entertainment System, Super Nintendo, Master System..

### Steps to reproduce the bug

1. Navigate to Online Updater
2. Select Thumbnails Updater - and any thumbnails pack
3. Task will fail.


### Version/Commit
Latest

- RetroArch: [version/commit]

### Environment information

- OS: [PSVita ]
- Compiler: [Precompiled Buildbot]


- [#4517](https://github.com/libretro/RetroArch/issues/4517) - open - XMB Horizontal browsing not smooth. - 13/08/2017

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

