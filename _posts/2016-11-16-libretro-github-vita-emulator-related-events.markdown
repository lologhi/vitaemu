---
layout: post
title:  "November 16th libretro updates concerning PS Vita emulation and emulators"
date:   2016-11-16 07:00:02 +0100
categories: vita emulation
---

### RetroArch
- [#3652](https://github.com/libretro/RetroArch/issues/3652) - closed - Built-in autoconfigs no longer working - 15/11/2016

I just tried this in windows, unzipped a fresh bundle, renamed autoconf dir. No input even though it said controller was detected.
I checked the settings and it was actually putting the settings in place but the controls don't work.
Renamed autoconf dir back and it works again.

It would be important to test this on other platforms like psp, vita, et al


- [#3010](https://github.com/libretro/RetroArch/issues/3010) - open - Thumbnail downloader issues - 15/11/2016

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


