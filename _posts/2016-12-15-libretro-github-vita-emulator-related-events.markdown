---
layout: post
title:  "December 15th libretro updates concerning PS Vita emulation and emulators"
date:   2016-12-15 06:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#4100](https://github.com/libretro/RetroArch/issues/4100) - open - PS Vita Overlay - 15/12/2016

Overlays on PS Vita don't respond to the touch screen.

- [#4026](https://github.com/libretro/RetroArch/issues/4026) - open - Vita: Will not save <Content dir> in directory for safefiles - 15/12/2016

Use the most recent nightly.  (I ran Nestopia core.)  Go into settings, directories.  Set the screenshot directory and savefile directory to some arbitrary directory.  Quit Retroarch.  Restart again and check the settings.  Both directories are set to the directory you chose.  Now change both of them to `<Content dir> `using the start button.  Quit Retroarch.  Restart again and check the settings.  Screenshot is still `<Content dir>`, but Savefile has forgotten the setting.

- [#4101](https://github.com/libretro/RetroArch/issues/4101) - closed - PS Vita MAME Menu - 15/12/2016

The R2 button don't exists on PS Vita, in the Mame Cores of PS Vita, the default button for MAME Menu is R2, I think it can be redefined by default to R1+L1, currently is not way to access to Dip Switches and Cheat menu.

- [#4092](https://github.com/libretro/RetroArch/issues/4092) - open - Execute Commandline Argument from Local File. - 15/12/2016

It would be useful to have Retroarch to check at startup briefly for stored commandline arguments in a file in the working directory (startup.cfg), and accept command line arguments stored there.  If detected, the command would be wiped from the file (so the command is not repeated) and then executed.

This would help sidestep an issue on systems with file system and application access, but cannot give command line arguments. Systems such as the Vita, PS3, and WiiU as well as future console or dedicated device ports may benefit from this. On systems without admin access to the OS to send commands to the executable, this would allow them to still utilize future Retroarch commands fully to launch directly into their content from other applications or interfaces, or into alternative display modes, etc.

### tyrquake
- [#30](https://github.com/libretro/tyrquake/pull/30) - open - (VITA) Fix build - 14/12/2016

