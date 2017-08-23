---
layout: post
title:  "August 23rd libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-23 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#4459](https://github.com/libretro/RetroArch/issues/4459) - closed - RetroArch will NOT "scan a directory" for MAME/FBA - 23/08/2017

Description:
Using "Scan Directory" on any FBA/MAME/etc. romset will not populate the menu with those ROMs.

Expected behavior:
I expect my clrmamePro verified ROMs (tried merged and non-merged romsets for 0.175 and 0.78) to show up in the menu underneath the MAME or FBA icon.

Actual behavior:
Nothing happens at all after scanning. Maybe 5-10 out of hundreds show up, but that's it.

Steps to reproduce the bug:
1. Load your MAME or FBA core of choice.
2. Go to the + and select "Scan Directory".
3. Select your directory where the matching (i.e. the correct romset for the core you selected in step one) romset ROMs are stored.
4. Select "Scan this Directory"
5. Once scanning is complete exit out to the main menu and notice only a few ROMs, or none at all, are listed under the appropriate MAME or FBA icon.

Bisect Results:
I've been trying this off and on for a full year (on all the recent 'stable' releases on RetroArch). I've tried it on a Windows 7 PC, Windows 10 PC, Mac running Yosemite, El Capitan, and Sierra, and a PS VIta and PSP (~10 computers/devices total)

Version/Commit
Neither "Version" or "Commit" are listed when I go into Information/System Information. 

RetroArch:
1.40

Environment information:
I've tried it on a Windows 7 PC, Windows 10 PC, Mac running Yosemite, El Capitan, and Sierra, and a PS VIta and PSP (~10 computers/devices total) - none will add more than a few ROMs to the menu.

Additional info:
These ROMs will load (with the correct core) if I select them individually - the problem is they simply will not be added to the menu under their system icon (unlike my NES/SNES/Sega Genesis, GBA, N64, etc. ROMs which all show up properly). Romsets are the most common type from archive-org and the like, and again, are verified with clrmamePro. I've been trying non-merged sets mainly, but this week I made merged sets for 0.78 and 0.175 and those do not work either. I've tried this on so many different computers and devices, running so many different OS's it's not even funny. I've made several different forum posts on several different forums and it seems like nobody can get this to work. Please let me know if there's anything I can do to test or provide more information and I will.



