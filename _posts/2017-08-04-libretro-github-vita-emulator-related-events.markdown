---
layout: post
title:  "August 04th libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-04 06:00:02 +0200
categories: vita emulation
---

### RetroArch
- [#5238](https://github.com/libretro/RetroArch/issues/5238) - open - Bounty to create/port an eBook reader core to Libretro/RetroArch - 03/08/2017

It has recently come to my attention that that no .epub readers exist for the PS Vita, and the only ebook reader exists that exists for the 3DS is currently abandoned. Indeed, ebook reader support tends to be sparse or inconsistent depending on the platform.

This is why I am creating a bounty for the creation/port of an ebBook reader core. Libretro's nature of being multi-platform allows it to easily deliver consistent experiences across cores.

Requirements:
.epub support
.pdf support
.cbz support
.mobi support
Has to be able to bookmark a page.
Controllable entirely with a controller
Has to be available on Windows, Linux, Android, Vita, and 3DS
I'll throw in some extra money for the bounty if OPDS support is added

I'd suggest porting either [CoolReader](https://sourceforge.net/projects/crengine/) or [FBReader](https://fbreader.org/) for this bounty. Both of these are licensed under GPL, so license issues shouldn't be a problem.


