---
layout: post
title:  "November 30th libretro updates concerning PS Vita emulation and emulators"
date:   2016-11-30 07:00:02 +0100
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


- [#4101](https://github.com/libretro/RetroArch/issues/4101) - open - PS Vita MAME Menu - 29/11/2016

The R2 button don't exists on PS Vita, in the Mame Cores of PS Vita, the default button for MAME Menu is R2, I think it can be redefined by default to R1+L1, currently is not way to access to Dip Switches and Cheat menu.

- [#4100](https://github.com/libretro/RetroArch/issues/4100) - open - PS Vita Overlay - 29/11/2016

Overlays on PS Vita don't respond to the touch screen.

- [#4099](https://github.com/libretro/RetroArch/issues/4099) - open - PS Vita thumbnails - 29/11/2016

The thumbnails don't work on PSVita.

- [#4092](https://github.com/libretro/RetroArch/issues/4092) - open - [Enhancement] [Request] Execute Commandline Argument from Local File. - 29/11/2016

It would be useful to have Retroarch to check at startup briefly for stored commandline arguments in a file in the working directory (startup.cfg), and accept command line arguments stored there.  If detected, the command would be wiped from the file (so the command is not repeated) and then executed.

This would help sidestep an issue on systems with file system and application access, but cannot give command line arguments. Systems such as the Vita, PS3, and WiiU as well as future console or dedicated device ports may benefit from this. On systems without admin access to the OS to send commands to the executable, this would allow them to still utilize future Retroarch commands fully to launch directly into their content from other applications or interfaces, or into alternative display modes, etc.

- [#3570](https://github.com/libretro/RetroArch/pull/3570) - open - Serial Scanning Removal for disk CRC scanning. - 29/11/2016

Removed the ISO and CUE serial scanning to prevent a conflict that will occur when the [disk CRC scanning](https://github.com/libretro/libretro-database/pull/251) is merged.


- [#3971](https://github.com/libretro/RetroArch/issues/3971) - open - Automatic Attract Mode - 29/11/2016

As RetroArch is moving into front end territory with individual game art etc I see a unique opportunity to go above and beyond what has been done before.

The most attractive front ends have not only static images but manually captured video files from individual games.

Most arcade games and many console games provide an "attract mode" that showcases the game when nobody is playing. If the core/rom was launched behind the front end as soon as a rom was in focus during game selection the output could be displayed as a non-interactive preview window. Input would still be routed to the front end at this point. Once a game is selected the front end could just zoom into the preview window and hand over input control to the core which would take over from there.

There would have to be some mechanism for the preview to quickly get to the point where the actual Attract Mode sequence starts. One way would be to speed up emulation until that point. A quicker way would be to have a special save state for when the Attract Mode sequence starts.

Games are usually sorted by system so there wouldn't be a need to reload a core as the user browses a collection. In most cases the same core would just reload a new rom.

This would provide a huge increase in visual attractiveness and usability without the need to download any media files related to individual roms. At most there would be a database of when attract mode starts for different games but just using best guesses would get us far. Any save states could be generated on the users machine.

