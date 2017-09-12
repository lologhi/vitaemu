---
layout: post
title:  "September 12th libretro updates concerning PS Vita emulation and emulators"
date:   2017-09-12 06:00:02 +0200
categories: vita emulation
---

### RetroArch
- [#5431](https://github.com/libretro/RetroArch/issues/5431) - open - [Vita] Can't set inputs R2/R3/L2/L3 in UI but manual retroarch.cfg edit works - 12/09/2017

## Description

The R2/R3/L2/L3 can not be set in the input settings.
Those buttons are somehow not detected by the emu.
Even enabling "touch" inputs.

The only option where "touch" inputs work is setting the Menu Toggle to L3+R3
Witch makes me think the emulator is detecting R2/R3/L2/L3 just fine.
But those are not enable to be set as the others inputs

**Edit-----**
Did some more testings and setting the buttons code in the Lastly retroarch.cfg works.
Things like **input_toggle_fast_forward_btn = "12"** works fine ingame.

So I think is only a issue in the UI that is ignoring R2/R3/L2/L3 as proper inputs.

### Expected behavior

I expect to be able to use R2/R3/L2/L3 to all the emu input options.
Like for hotkeys or PS1 games that required R2/R3/L2/L3

### Actual behavior

There is no way to use R2/R3/L2/L3 for inputs.
But Menu Toggle L3+R3 works fine

### Steps to reproduce the bug

Go into the input menu.
Chose a hotkey and try to set it to  R2/R3/L2/L3.

### Version/Commit
Tested on nighly 04/09


