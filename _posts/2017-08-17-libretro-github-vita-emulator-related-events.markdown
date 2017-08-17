---
layout: post
title:  "August 17th libretro updates concerning PS Vita emulation and emulators"
date:   2017-08-17 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#5293](https://github.com/libretro/RetroArch/issues/5293) - open - 1.6.4 PS Vita - Online Updater - Thumbnails Updater fails - 16/08/2017


## Description
Using Retroarch 1.6.4 for PS Vita, Thumbnails Updater fails. 

### Expected behavior

Thumbnails Updater should download and extract selected thumbnails to directory 

### Actual behavior

Thumbnails download will get to about 50%, than restart itself - showing text indicating 0% before finally failing with 'Task Failed'.


Tested with Mega Drive, Nintendo - Nintendo Entertainment System, Super Nintendo, Master System..

### Steps to reproduce the bug

1. Navigate to Online Updater
2. Select Thumbnails Updater - and any thumbnails pack
3. Task will fail.


### Version/Commit
Latest

- RetroArch: [version/commit]

### Environment information

- OS: [PSVita ]
- Compiler: [Precompiled Buildbot]


