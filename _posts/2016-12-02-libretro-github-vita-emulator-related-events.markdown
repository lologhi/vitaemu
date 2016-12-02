---
layout: post
title:  "December 02nd libretro updates concerning PS Vita emulation and emulators"
date:   2016-12-02 07:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#4126](https://github.com/libretro/RetroArch/pull/4126) - closed - inet_ntoa missing on Vita - 02/12/2016

It's hard to know exactly how lacking SOCKET_LEGACY is, but evidently Vita doesn't support inet_ntoa, so I guess the poor SOCKET_LEGACY bastards don't get to know what their public IP address is.

- [#4113](https://github.com/libretro/RetroArch/pull/4113) - closed - Adding NAT traversal announcement for SOCKET_LEGACY - 01/12/2016

This should fix the Vita Netplay build.

