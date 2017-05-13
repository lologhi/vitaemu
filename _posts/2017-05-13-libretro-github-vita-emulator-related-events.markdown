---
layout: post
title:  "May 13th libretro updates concerning PS Vita emulation and emulators"
date:   2017-05-13 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - closed - Vita testing - 12/05/2017

20/01/2017 - Announcement:
I"m now reporting issues in separated reports.
Maybe this way it gets a bit more attention.
So I'll not update this report any longer.

---------------------------------------------------------------------------------------
Old report :
---------------------------------------------------------------------------------------
~~I'll be posting the vita issues found in my testings here.
When issue is fixed the main post will be updated.
If this is not the appropriate place for this report please let me know.~~

21/11/16 - System is now on TaiHenkaku.
18/01/17 - Retroarch on beta 1.40

General issues:
1-  ~~Saving state first shows text "loading state" (0-100%) them "saving state" (0-100%)
Started to happen some nightlys ago. Can't finda the exact one since only the last 5 are available.
(Improved a lot on 1.40 but is still noticible on PSX ReARMed)~~ **RA issue not related to the vita**

2- ~~Frame Trottle is disable/not working
It was working in the early nightlys (Maybe this one was intentionally disabled for stability)
(Still not working with 1.40)~~ **Fixed in 11/05/17**

3- ~~Scan directory cause the app to crash. (probably is not fully implemented yet)~~ -**Fixed 14/10/16**

4- ~~Performance while on menus dropped a bit. Folder scanning is also a lot slower.~~ -**Fixed 18/01/17**

5- ~~While running a game in the background is not possible to load another in the system scanned list.
The loaded game is always the first one.~~**Fixed in 11/05/17**

Per-Core issues
1 - GPSP - Random Stutter - Apparently this issues started after the Dynarec update.
(Problem persists in 1.40)


