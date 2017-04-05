---
layout: post
title:  "April 05th libretro updates concerning PS Vita emulation and emulators"
date:   2017-04-05 06:00:01 +0200
categories: vita emulation
---

### RetroArch
- [#4799](https://github.com/libretro/RetroArch/issues/4799) - open - [Vita] Mega Drive II roms only shown if 7zipped - 04/04/2017

On my Vita, RetroArch is only showing 7zipped Mega Drive II roms. Zipped and plain are ignored.
I've tried RetroArch 1.5.0 and nightly 2017-04-04, same result. 1.5.0 on Windows shows all formats.
See attached screenshots of RetroArch and VitaShell.
![vitashell](https://cloud.githubusercontent.com/assets/1146987/24678911/58a67884-1984-11e7-9ad4-668df4619f72.jpg)
![retroarch](https://cloud.githubusercontent.com/assets/1146987/24678910/58a63946-1984-11e7-961e-a655b5fdf9eb.jpg)



<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/43793525-vita-mega-drive-ii-roms-only-shown-if-7zipped?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4800](https://github.com/libretro/RetroArch/issues/4800) - open - Question: How are zip/7z files processed? - 05/04/2017

On my Vita, scanning them seems quite slow, so I'm wondering if they're unpacked to a temp directory to check the hash?
Checking the CRC doesn't require unpacking, it can be read from the archive headers.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/43797234-question-how-are-zip-7z-files-processed?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

- [#4461](https://github.com/libretro/RetroArch/issues/4461) - open - Frame Trottle is disable/not working - 04/04/2017

As of 1.40 Frame Trottle is still not working.
It was working in the early Vita releases back when Henkaku became popular but somehow it got disable.

<bountysource-plugin>

---
Want to back this issue? **[Post a bounty on it!](https://www.bountysource.com/issues/41152998-frame-trottle-is-disable-not-working?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github)** We accept bounties via [Bountysource](https://www.bountysource.com/?utm_campaign=plugin&utm_content=tracker%2F296058&utm_medium=issues&utm_source=github).
</bountysource-plugin>

