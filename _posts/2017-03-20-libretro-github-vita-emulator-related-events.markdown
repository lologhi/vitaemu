---
layout: post
title:  "March 20th libretro updates concerning PS Vita emulation and emulators"
date:   2017-03-20 06:00:02 +0100
categories: vita emulation
---

### RetroArch
- [#3793](https://github.com/libretro/RetroArch/issues/3793) - open - Vita testing - 19/03/2017

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


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/38378351-vita-testing?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4100](https://github.com/libretro/RetroArch/issues/4100) - open - PS Vita Overlay - 19/03/2017

Overlays on PS Vita don't respond to the touch screen.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/39791670-ps-vita-overlay?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3435](https://github.com/libretro/RetroArch/issues/3435) - open - Native vita keyboard - 19/03/2017

Would it be possible/feasible to use the native vita keyboard by calling psp2/ime_dialogue.h from https://github.com/vitasdk/vita-headers and grabbing that input, instead of using the RA input system?


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/37317896-native-vita-keyboard?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4752](https://github.com/libretro/RetroArch/issues/4752) - open - Add cheevos/retroachivements to Vita port - 19/03/2017

Could we please benefit from being able to connect to RetroAchievement on the Vita builds of RetroArch?

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/42986620-add-cheevos-retroachivements-to-vita-port?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4699](https://github.com/libretro/RetroArch/issues/4699) - open - [ps vita] content mount points broken - 19/03/2017

## Description

In the last stable build 1.4.1, when selecting Load Content, the ps vita mount points (ux0, app0,...) were selectable. Now only the mount point / is proposed but cannot be used on the vita.

### Expected behavior

Possible to select vita mount points (especially ux0) from Load Content

### Actual behavior

Only a not working mount point "/" is proposed

### Steps to reproduce the bug

1. Select Load Content menu

### Version/Commit

- RetroArch: current master

### Environment information

- OS: ps vita
- Compiler: libretro nightly builds


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/42444335-ps-vita-content-mount-points-broken?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3841](https://github.com/libretro/RetroArch/issues/3841) - open - PS VITA Handy core issue - 19/03/2017

Emulator immediately crashes upon loading new ROM with Handy core loaded.  10/20 AIO build.  

edit - The first ROM loaded is fine, its when you try to load a different ROM within same session it crashes.


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/38582806-ps-vita-handy-core-issue?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4026](https://github.com/libretro/RetroArch/issues/4026) - open - Vita: Will not save <Content dir> in directory for safefiles - 19/03/2017

Use the most recent nightly.  (I ran Nestopia core.)  Go into settings, directories.  Set the screenshot directory and savefile directory to some arbitrary directory.  Quit Retroarch.  Restart again and check the settings.  Both directories are set to the directory you chose.  Now change both of them to `<Content dir> `using the start button.  Quit Retroarch.  Restart again and check the settings.  Screenshot is still `<Content dir>`, but Savefile has forgotten the setting.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/39410015-vita-will-not-save-content-dir-in-directory-for-safefiles?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3854](https://github.com/libretro/RetroArch/issues/3854) - open - Binding L2/3 and R2/3 to hotkeys VITA - 19/03/2017

It appears you cannot bind turbo or any hotkeys to L2/3 and R2/3 when touch screen / touch screen front preferred enabled.  

Would be immensely useful if implemented.


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/38649370-binding-l2-3-and-r2-3-to-hotkeys-vita?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3850](https://github.com/libretro/RetroArch/issues/3850) - open - PS Vita Retroarch Unable to Open after Choosing wrong BIOS - 19/03/2017

So on accident earlier, I had loaded a PS1 BIOS, which caused retroarch to be stuck in a boot loop where it would continuously return to the live area every time retroarch is to be opened.

It was only after I had deleted the core config file that the issue was fixed. Would be nice if this was raised up in case others had ended up doing the same as I had and save them some time.


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/38615542-ps-vita-retroarch-unable-to-open-after-choosing-wrong-bios?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4461](https://github.com/libretro/RetroArch/issues/4461) - open - Frame Trottle is disable/not working - 19/03/2017

As of 1.40 Frame Trottle is still not working.
It was working in the early Vita releases back when Henkaku became popular but somehow it got disable.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/41152998-frame-trottle-is-disable-not-working?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4460](https://github.com/libretro/RetroArch/issues/4460) - open - UI issue - Saving state shows text "loading state" them "saving state" - 19/03/2017

Small annoying issue were saving first shows text "loading state" (0-100%) them "saving state" (0-100%).
Tested on 1.40.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/41152949-ui-issue-saving-state-shows-text-loading-state-them-saving-state?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4092](https://github.com/libretro/RetroArch/issues/4092) - open - Execute Commandline Argument from Local File. - 19/03/2017

It would be useful to have Retroarch to check at startup briefly for stored commandline arguments in a file in the working directory (startup.cfg), and accept command line arguments stored there.  If detected, the command would be wiped from the file (so the command is not repeated) and then executed.

This would help sidestep an issue on systems with file system and application access, but cannot give command line arguments. Systems such as the Vita, PS3, and WiiU as well as future console or dedicated device ports may benefit from this. On systems without admin access to the OS to send commands to the executable, this would allow them to still utilize future Retroarch commands fully to launch directly into their content from other applications or interfaces, or into alternative display modes, etc.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/39604264-execute-commandline-argument-from-local-file?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4517](https://github.com/libretro/RetroArch/issues/4517) - open - XMB Horizontal browsing not smooth. - 19/03/2017

When you have multiple playlists and some of them are huge, XMB will halt on them.

Keeping the right direction pushed down will stop the browsing for a while on my big Mame playlist (5s).
To speed it up a bit I have to release the direction, and try to push again several times until it moves.
If I don't the browsing will get really slow at proceeding through every item (1s-2s each).

That's an extreme case playlist of 75000+ lines but 10000 lines (complete romset of many systems) is enough to make strong hiccups.

Would it be possible to limit the entries loaded when simply browsing left-right to optimize this?

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/41393572-xmb-horizontal-browsing-not-smooth?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3010](https://github.com/libretro/RetroArch/issues/3010) - open - Thumbnail downloader issues - 19/03/2017

Had a conversation last night with leiradel and we concluded the current approach won't scale.
The conversation:
http://hastebin.com/odocajumog.xml

So, monolithic download pros:
- single download, should be faster if the user wants all the thumbs since it would mean less requests
- virtually zero infrastructure changes
- once unzipped, it's done, just works

monolithic download cons:
- huge file, should take a while to download and extract, many users will hammer the download every week or so even if there are no changes, wasting our bandwidth and killing their storage on the way

On-demand download pros:
- small downloads, should take just a few seconds per-thumbnail on a decent connection
- acts like a cache, once a file is fetched it wouldn't be downloaded
- again no infraestructure changes
- if a file is added it could be updated without downloading 300MB again
- can be cached by a CDN making the bandwidth requirement on server side virtually zero
- the approach could scale to download cheats, icons, saves, patches, anything we want

On-demand download cons:
- noticeable delay before a thumbnail appears (the first time), same thing happens virtually anywhere, heck even loading the thumbnails from the cache on steam takes a couple seconds
- more code needed on the RetroArch side
- needs a few alterations to the OSD interface to avoid spamming messages

Anyway, my $0.02, it would be up to you guys, I just thought I should make a list and try to weigh pros and cons.

@Kivutar @leiradel @twinaphex 


<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/34335268-thumbnail-downloader-issues?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#3971](https://github.com/libretro/RetroArch/issues/3971) - open - Automatic Attract Mode - 19/03/2017

As RetroArch is moving into front end territory with individual game art etc I see a unique opportunity to go above and beyond what has been done before.

The most attractive front ends have not only static images but manually captured video files from individual games.

Most arcade games and many console games provide an "attract mode" that showcases the game when nobody is playing. If the core/rom was launched behind the front end as soon as a rom was in focus during game selection the output could be displayed as a non-interactive preview window. Input would still be routed to the front end at this point. Once a game is selected the front end could just zoom into the preview window and hand over input control to the core which would take over from there.

There would have to be some mechanism for the preview to quickly get to the point where the actual Attract Mode sequence starts. One way would be to speed up emulation until that point. A quicker way would be to have a special save state for when the Attract Mode sequence starts.

Games are usually sorted by system so there wouldn't be a need to reload a core as the user browses a collection. In most cases the same core would just reload a new rom.

This would provide a huge increase in visual attractiveness and usability without the need to download any media files related to individual roms. At most there would be a database of when attract mode starts for different games but just using best guesses would get us far. Any save states could be generated on the users machine.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/39121614-automatic-attract-mode?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

