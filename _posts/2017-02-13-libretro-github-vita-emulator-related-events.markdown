---
layout: post
title:  "February 13th libretro updates concerning PS Vita emulation and emulators"
date:   2017-02-13 06:00:02 +0100
categories: vita emulation
---

### pcsx_rearmed
- [#40](https://github.com/libretro/pcsx_rearmed/issues/40) - open - [RPI2] [BUG] MGS Graphic Glitch - 12/02/2017

This issue is pretty easy to reproduce. Instead of the white flash which usually opens a cut scene there is a pixel mess with a kind of stroboscopic effect. Really weird. Let me attach a screenshot as it's worth a thousand words I guess. The first time to see this it's right after the lift, after Snake takes his swimsuit off. It appears again just a few seconds later when Snake stares at the Hind-D.

I'm using a RP2, latest Retropie version (3.7 final), this core freshly built (but same behavior with the other rearmed core). Core options all by default/auto. No video enhancement turned on or something. I'm using bios SCPH1001.BIN but it makes no difference as same behavior occurs with any other bioses.

As french I'm playing with the FR version of the game (not the Integral or Special version of the game). Didn't try with another version but I could do so if that helps.

Thanks for your help and assistance.

![54a8b63a-5035-11e5-9423-056e2b85e2f8](https://cloud.githubusercontent.com/assets/8100500/15267446/b57fb48e-19c2-11e6-839a-4c9a78600f42.png)


