---
layout: post
title:  "December 06th libretro updates concerning PS Vita emulation and emulators"
date:   2016-12-06 07:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - open - Vita testing - 05/12/2016

I'll be posting the vita issues found in my testings here.
When issue is fixed the main post will be updated.
If this is not the appropriate place for this report please let me know.

As of 21/11 all testings are on TaiHenkaku.

General issues:
1-  Saving state first shows text "loading state" (0-100%) them "saving state" (0-100%)
Started to happen some nightlys ago. Can't finda the exact one since only the last 5 are available.

2- Frame Trottle is disable/not working
It was working in the early nightlys (Maybe this one was intentionally disabled for stability)

3- ~~Scan directory cause the app to crash. (probably is not fully implemented yet)~~ -**Fixed 14/10**

4- Performance while on menus droped a bit. Folder scanning is also a lot slower.

5- While running a game in the background is not possible to load another in the system scanned list.
The loaded game is always the first one.

Per-Core issues
1 - GPSP - Random Stutter - Apparently this issues started after the Dynarec update.


