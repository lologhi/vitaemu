---
layout: post
title:  "March 19th libretro updates concerning PS Vita emulation and emulators"
date:   2017-03-19 06:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#4699](https://github.com/libretro/RetroArch/issues/4699) - open - [ps vita] content mount points broken - 18/03/2017

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


