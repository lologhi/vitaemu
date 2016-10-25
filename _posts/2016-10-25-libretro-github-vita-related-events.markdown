---
layout: post
title:  "October 25th libretro updates concerning PS Vita"
date:   2016-10-25 10:00:00 +0800
categories: vita emulation
---

### RetroArch
- [#3850](https://github.com/libretro/RetroArch/issues/3850) - open - PS Vita Retroarch Unable to Open after Choosing wrong BIOS - 24/10/2016

So on accident earlier, I had loaded a PS1 BIOS, which caused retroarch to be stuck in a boot loop where it would continuously return to the live area every time retroarch is to be opened.

It was only after I had deleted the core config file that the issue was fixed. Would be nice if this was raised up in case others had ended up doing the same as I had and save them some time.
