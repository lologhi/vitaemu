---
layout: post
title:  "November 29th libretro updates concerning PS Vita emulation and emulators"
date:   2016-11-29 07:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - open - Vita testing - 29/11/2016

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


- [#4092](https://github.com/libretro/RetroArch/issues/4092) - open - [Enhancement] [Request] Execute Commandline Argument from Local File. - 29/11/2016

It would be useful to have Retroarch to check at startup briefly for stored commandline arguments in a file in the working directory (startup.cfg), and accept command line arguments stored there.  If detected, the command would be wiped from the file (so the command is not repeated) and then executed.

This would help sidestep an issue on systems with file system and application access, but cannot give command line arguments. Systems such as the Vita, PS3, and WiiU as well as future console or dedicated device ports may benefit from this. On systems without admin access to the OS to send commands to the executable, this would allow them to still utilize future Retroarch commands fully to launch directly into their content from other applications or interfaces, or into alternative display modes, etc.

