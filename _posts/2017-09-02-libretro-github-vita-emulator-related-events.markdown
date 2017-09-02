---
layout: post
title:  "September 02nd libretro updates concerning PS Vita emulation and emulators"
date:   2017-09-02 06:00:01 +0200
categories: vita emulation
---

### pcsx_rearmed
- [#103](https://github.com/libretro/pcsx_rearmed/issues/103) - open - Far polygons are broken when usng arm dynarec - 01/09/2017

The polygon culling on the arm dynarec completely destroys long distance objects, I tested with pcsx-rearmed android, pcsx-rearmed mac and openemu mednafen.
Only pcsx-rearmed android was effected.
Here is an archive of all test screenshots plus 2 broken ones for easy viewing.
[neonremove.zip](https://github.com/libretro/pcsx_rearmed/files/785305/neonremove.zip)
![ctr - crash team racing usa -170218-122200](https://cloud.githubusercontent.com/assets/1220805/23096746/b71e9c28-f5d7-11e6-91fc-f28083720cf0.png)
![ctr - crash team racing usa -170218-122108](https://cloud.githubusercontent.com/assets/1220805/23096747/ba878762-f5d7-11e6-9619-d971e7639c97.png)

I originally thought it was the fault of the neon gpu plugin but after using unai gpu on android and testing it it still happened so all thats left is the dynarec.




<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/42186176-far-polygons-are-broken-when-usng-arm-dynarec?utm_campaign=plugin&utm_content=tracker%2F441984&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F441984&utm_medium=issues&utm_source=github).
</bountysource-plugin>

