---
layout: post
title:  "November 22nd libretro updates concerning PS Vita emulation and emulators"
date:   2016-11-22 07:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - open - Vita testing - 21/11/2016

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
(Still testing cores so this section might take a while)


- [#4026](https://github.com/libretro/RetroArch/issues/4026) - open - Vita: Will not save <Content dir> in directory for safefiles - 21/11/2016

Use the most recent nightly.  (I ran Nestopia core.)  Go into settings, directories.  Set the screenshot directory and savefile directory to some arbitrary directory.  Quit Retroarch.  Restart again and check the settings.  Both directories are set to the directory you chose.  Now change both of them to `<Content dir> `using the start button.  Quit Retroarch.  Restart again and check the settings.  Screenshot is still `<Content dir>`, but Savefile has forgotten the setting.

- [#4027](https://github.com/libretro/RetroArch/issues/4027) - open - Nonsensical PAR/DAR description - 21/11/2016

Start without a core.  Go into video, Aspect Ratio Index.  One of the options is "1:1 PAR (4:3 DAR)".  Since no core is loaded, there is no way for Retroarch to know that 1:1 PAR corresponds to 4:3 DAR and, in fact, this correspondence is not true for some cores.

It also does the same thing with a core, without checking to see if the core is one for which 1:1 PAR is 4:3 DAR (for instance, it is not true for Nestopia.)


