---
layout: post
title:  "Last libretro updates for PS Vita"
date:   2016-10-24 00:31:00 +0800
categories: vita emulation
---

I've just coded a small script using Github API to retrieve recent updates concerning PS Vita in all libretro repos. Here is the first result on the four last days. I intend to update this every day :)

### RetroArch
- [#3841](https://github.com/libretro/RetroArch/issues/3841) - PS VITA Handy core issue - 22/10/2016

Emulator immediately crashes upon loading new ROM with Handy core loaded.  10/20 AIO build.

edit - The first ROM loaded is fine, its when you try to load a different ROM within same session it crashes.

- [#3830](https://github.com/libretro/RetroArch/issues/3830) - (VITA) FBA cheat support - 20/10/2016

I would like to ask if is possible to add the cheat support (.ini file) for FBA in future updates, like the real FBA allow...
Many games enable more game options over the common cheating as well (like playing as a bosses in SF games)

- [#3833](https://github.com/libretro/RetroArch/issues/3833) - (Vita) FBA CPS1, CPS2 and NeoGeo NVRAM Save Files - 20/10/2016

Under MAME2003, this Core Creates NVRAM Saves, but the FBA Cores do not. Which means any Settings that are changed, have to keep getting Changed every time you select a certain Game.
Example:
HSF2
Go into System Menu and Select Free Play, Demo Sound On, Change Difficulty Settings, ect.

- [#3828](https://github.com/libretro/RetroArch/issues/3828) - (VITA-FBA-gpsp)Since build 18.10.2016 Crashes on Rom load - 20/10/2016

When we load a Rom via fbalpha or gpsp core (maybe more, untested) on every build since 18.10.2016, it crashes with a dump
This happens every time.

Bios is placed in: UX0:/data/retroarch/system
Proper system path is set in Retroarch

Versions tested: 18.10.2016 Nightly and up
All under 18.10 don't suffer from this bug.


The dump is renamed to .zip to allow upload. Please rename it back to .psp2dmp
[psp2core-1476881151-0x00010e310f-fbalpha_libretro.self.zip](https://github.com/libretro/RetroArch/files/539148/psp2core-1476881151-0x00010e310f-fbalpha_libretro.self.zip)


### vba-next
- [#70](https://github.com/libretro/vba-next/pull/70) - (VITA) Updated Makefile. - 12/10/2016

- [#69](https://github.com/libretro/vba-next/pull/69) - (VITA) Updated Makefile. - 12/10/2016

- [#68](https://github.com/libretro/vba-next/pull/68) - (VITA) Updated Makefile. - 12/10/2016

- [#67](https://github.com/libretro/vba-next/pull/67) - (VITA) Updated Makefile. - 12/10/2016

### mame2000-libretro
- [#28](https://github.com/libretro/mame2000-libretro/pull/28) - (VITA) Fix - 18/09/2016

### pcsx_rearmed
- [#69](https://github.com/libretro/pcsx_rearmed/issues/69) - Tried pcsx on vita but gets error (C2-12828-1). - 26/09/2016

As you see on the title I got error when I want to try play ps1 games.

It said when I select game: error(C2-12828-1) saved core file succeeded ux0/data/psp2core-1474853369-0x00000730fb-eboot.bin.psp2dmp.

Any solution please?

- [#75](https://github.com/libretro/pcsx_rearmed/pull/75) - (VITA) Use RWX path - 04/10/2016

- [#68](https://github.com/libretro/pcsx_rearmed/pull/68) - (VITA) Dynarec working - 25/09/2016

- [#70](https://github.com/libretro/pcsx_rearmed/pull/70) - Fix build error about undefined reference to `deinit_vita_mmap' - 26/09/2016

```
frontend/libretro.o: In function `retro_deinit':
libretro.c:(.text+0x3769): undefined reference to `deinit_vita_mmap'
collect2: error: ld returned 1 exit status
make: *** [pcsx_rearmed_libretro.so] Error 1
```
Introduced #68

- [#61](https://github.com/libretro/pcsx_rearmed/pull/61) - (VITA) I think this is not going to work but if someone can test it - 07/09/2016

### dosbox-libretro
- [#42](https://github.com/libretro/dosbox-libretro/pull/42) - (VITA) Fix O3 and core options - 28/09/2016

### mame2003-libretro
- [#64](https://github.com/libretro/mame2003-libretro/pull/64) - (Vita) Add O3 optimizations - 27/09/2016

- [#56](https://github.com/libretro/mame2003-libretro/pull/56) - (VITA) Initial build with -O0 - 27/08/2016

Got this working with -O0

Got not time to do more test with -O1, etc

You can add it to the rest of cores

### tyrquake
- [#20](https://github.com/libretro/tyrquake/pull/20) - VIta working now - 17/09/2016

- [#19](https://github.com/libretro/tyrquake/pull/19) - (VITA) Move some stack memory to heap - 14/09/2016
