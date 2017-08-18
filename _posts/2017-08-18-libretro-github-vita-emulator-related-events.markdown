---
layout: post
title:  "August 18th libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-18 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#5317](https://github.com/libretro/RetroArch/issues/5317) - closed - Stuttering on nes games -psvita - 17/08/2017

Using retroarch on the psvita, Have check to make sure its not a core issue but one to do with retroarch by testing all the cores and the problem persists. 
retroarch git version:47cf178
Compiler:(6.2.0) 32-bit 

[Description of the bug]
When playing Pal games on the NES there is a persistent  stuttering and graphical glitch when the screen is scrolling fast and there is a few sprites on screen, while this happens the sound also has a stutter.
while this happens the fps stays consistent witch makes me think its a refresh rate issue.
I have tried to use the in built menu to change this like turning of vsync ect, but no matter what option int he quick menu or video menu I use will change this.
Because the PAL version of the NES run at 50Hz i tried a NTSC version of the same rom and it worked alot better witch makes me think I was right with it being a refresh rate issue.

[Steps to reproduce the bug}

1. run super mario on the nes retroarch for ps vita
2. in world 2-1 after the first pipe run along the ? blocks as fast as you can and shoot fire until the next pipe

this happens alot throughout the game but that is the only spot I can reproduce the issue consistently. 




