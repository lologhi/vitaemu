---
layout: post
title:  "November 23rd libretro updates concerning PS Vita emulation and emulators"
date:   2016-11-23 07:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#4026](https://github.com/libretro/RetroArch/issues/4026) - open - Vita: Will not save <Content dir> in directory for safefiles - 22/11/2016

Use the most recent nightly.  (I ran Nestopia core.)  Go into settings, directories.  Set the screenshot directory and savefile directory to some arbitrary directory.  Quit Retroarch.  Restart again and check the settings.  Both directories are set to the directory you chose.  Now change both of them to `<Content dir> `using the start button.  Quit Retroarch.  Restart again and check the settings.  Screenshot is still `<Content dir>`, but Savefile has forgotten the setting.

- [#4027](https://github.com/libretro/RetroArch/issues/4027) - closed - Nonsensical PAR/DAR description - 22/11/2016

Start without a core.  Go into video, Aspect Ratio Index.  One of the options is "1:1 PAR (4:3 DAR)".  Since no core is loaded, there is no way for Retroarch to know that 1:1 PAR corresponds to 4:3 DAR and, in fact, this correspondence is not true for some cores.

It also does the same thing with a core, without checking to see if the core is one for which 1:1 PAR is 4:3 DAR (for instance, it is not true for Nestopia.)


