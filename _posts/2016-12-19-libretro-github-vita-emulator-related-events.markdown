---
layout: post
title:  "December 19th libretro updates concerning PS Vita emulation and emulators"
date:   2016-12-19 06:00:02 +0100
categories: vita emulation
---

### RetroArch
- [#4092](https://github.com/libretro/RetroArch/issues/4092) - open - Execute Commandline Argument from Local File. - 18/12/2016

It would be useful to have Retroarch to check at startup briefly for stored commandline arguments in a file in the working directory (startup.cfg), and accept command line arguments stored there.  If detected, the command would be wiped from the file (so the command is not repeated) and then executed.

This would help sidestep an issue on systems with file system and application access, but cannot give command line arguments. Systems such as the Vita, PS3, and WiiU as well as future console or dedicated device ports may benefit from this. On systems without admin access to the OS to send commands to the executable, this would allow them to still utilize future Retroarch commands fully to launch directly into their content from other applications or interfaces, or into alternative display modes, etc.

- [#3570](https://github.com/libretro/RetroArch/pull/3570) - open - Serial Scanning Removal for disk CRC scanning. - 18/12/2016

Removed the ISO and CUE serial scanning to prevent a conflict that will occur when the [disk CRC scanning](https://github.com/libretro/libretro-database/pull/251) is merged.


