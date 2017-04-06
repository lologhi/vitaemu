---
layout: post
title:  "April 06th libretro updates concerning PS Vita emulation and emulators"
date:   2017-04-06 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#4801](https://github.com/libretro/RetroArch/pull/4801) - closed - [VITA] Fix slow IO - 05/04/2017

- [#4800](https://github.com/libretro/RetroArch/issues/4800) - closed - Question: How are zip/7z files processed? - 05/04/2017

On my Vita, scanning them seems quite slow, so I'm wondering if they're unpacked to a temp directory to check the hash?
Checking the CRC doesn't require unpacking, it can be read from the archive headers.

### vba-next
- [#81](https://github.com/libretro/vba-next/issues/81) - open - [Vita] Saving state crashes Vita - 05/04/2017

Attempting to save the state crashes the Vita's OS.
It gets to 98/99% and then I get:
```
An error has occurred.
The PS Vita system will be powered off.
```
RetroArch nightly 2017-04-04

Doesn't seem to be game specific. I've tried Pokemon LeafGreen and Pokemon Emerald, same result.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/43834629-vita-saving-state-crashes-vita?utm_campaign=plugin&utm_content=tracker%2F1027743&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F1027743&utm_medium=issues&utm_source=github).
</bountysource-plugin>

