---
layout: post
title:  "January 21st libretro updates concerning PS Vita emulation and emulators"
date:   2017-01-21 06:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - open - Vita testing - 20/01/2017

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
1-  Saving state first shows text "loading state" (0-100%) them "saving state" (0-100%)
Started to happen some nightlys ago. Can't finda the exact one since only the last 5 are available.
(Improved a lot on 1.40 but is still noticible on PSX ReARMed)

2- Frame Trottle is disable/not working
It was working in the early nightlys (Maybe this one was intentionally disabled for stability)
(Still not working with 1.40)

3- ~~Scan directory cause the app to crash. (probably is not fully implemented yet)~~ -**Fixed 14/10/16**

4- ~~Performance while on menus dropped a bit. Folder scanning is also a lot slower.~~ -**Fixed 18/01/17**

5- While running a game in the background is not possible to load another in the system scanned list.
The loaded game is always the first one.

Per-Core issues
1 - GPSP - Random Stutter - Apparently this issues started after the Dynarec update.
(Problem persists in 1.40)


- [#4461](https://github.com/libretro/RetroArch/issues/4461) - open - [Vita] Frame Trottle is disable/not working - 20/01/2017

As of 1.40 Frame Trottle is still not working.
It was working in the early Vita releases back when Henkaku became popular but somehow it got disable.

- [#4462](https://github.com/libretro/RetroArch/issues/4462) - closed - [Vita] GPSP Core Random Stuttering - 20/01/2017

This issue started with the release of a dynarec update/patch for this core.
The core will stutter randomly causing audio and video lagging. 
Problem still persists in 1.40.

- [#4460](https://github.com/libretro/RetroArch/issues/4460) - open - UI issue - Saving state shows text "loading state" them "saving state" - 20/01/2017

Small annoying issue were saving first shows text "loading state" (0-100%) them "saving state" (0-100%).
Tested on 1.40.

- [#4459](https://github.com/libretro/RetroArch/issues/4459) - open - RetroArch will NOT "scan a directory" for MAME/FBA - 21/01/2017

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



### pcsx_rearmed
- [#92](https://github.com/libretro/pcsx_rearmed/issues/92) - open - [Vita] pcsx_rearmed saving states is extremely slow - 20/01/2017

So saving stats or loading is really really slow in pcsx_rearmed.
Also saving cause a very strong slowdown and lagging of the game.

Tested on 1.40.
Other cores are behaving better like Snes2005 and GPSP

- [#91](https://github.com/libretro/pcsx_rearmed/issues/91) - open - [Vita] pcsx_rearmed will stop working after Sleep-Mode - 20/01/2017

So the pcsx_rearmed core will freeze and sometimes loose audio and lagg after the vita enters sleep mode.

This behavior does not happen on Snes2005 or Gpsp.
So I think is core related.
Tested on 1.40

