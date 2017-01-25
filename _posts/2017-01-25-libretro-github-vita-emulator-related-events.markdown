---
layout: post
title:  "January 25th libretro updates concerning PS Vita emulation and emulators"
date:   2017-01-25 06:00:02 +0100
categories: vita emulation
---

### pcsx_rearmed
- [#89](https://github.com/libretro/pcsx_rearmed/issues/89) - open - questions about 3DS port - 24/01/2017

* It's missing from nightly for a while, I actually doesn't have a build on my hand, does anyone have a working build?
* retroarch on 3DS show the core name as PCSX, not PCSX-ReARMed, is it just cosmetic or actually a different core? I haven't found a PCSX repo on https://github.com/libretro/, only this.
* I'm guessing the speed difference between 3DS and Vita is NEON support, despite on a much higher frequency, 3DS CPU doesn't support NEON, and PCSX-ReARMed probably used the NEON GPU in Vita builds, is that right?
* I want to help improve PCSX on 3DS, I'm a programmer, have some C experience but I know pretty much nothing about emulation, where should I look into?

I prefer PSX on 3DS over Vita, despite the inferior screen, the resolution is just enough for PSX, and the pixelating gives a *genuine* nostalgic feeling. and it has ZL/ZR for L2/R2!

- [#40](https://github.com/libretro/pcsx_rearmed/issues/40) - open - [RPI2] [BUG] MGS Graphic Glitch - 24/01/2017

This issue is pretty easy to reproduce. Instead of the white flash which usually opens a cut scene there is a pixel mess with a kind of stroboscopic effect. Really weird. Let me attach a screenshot as it's worth a thousand words I guess. The first time to see this it's right after the lift, after Snake takes his swimsuit off. It appears again just a few seconds later when Snake stares at the Hind-D.

I'm using a RP2, latest Retropie version (3.7 final), this core freshly built (but same behavior with the other rearmed core). Core options all by default/auto. No video enhancement turned on or something. I'm using bios SCPH1001.BIN but it makes no difference as same behavior occurs with any other bioses.

As french I'm playing with the FR version of the game (not the Integral or Special version of the game). Didn't try with another version but I could do so if that helps.

Thanks for your help and assistance.

![54a8b63a-5035-11e5-9423-056e2b85e2f8](https://cloud.githubusercontent.com/assets/8100500/15267446/b57fb48e-19c2-11e6-839a-4c9a78600f42.png)


