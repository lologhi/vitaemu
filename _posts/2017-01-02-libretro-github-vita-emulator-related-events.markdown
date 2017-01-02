---
layout: post
title:  "January 02nd libretro updates concerning PS Vita emulation and emulators"
date:   2017-01-02 06:00:01 +0100
categories: vita emulation
---

### RetroArch
- [#3843](https://github.com/libretro/RetroArch/issues/3843) - closed - Several Cores Crash When input_max_users Set < 5 - 01/01/2017

I'm getting a crash with this core when loading content on today's nightly (10/22). It doesn't happen in the previous one available on the buildbot (10/20). A bt in gdb gives me:

> Program received signal SIGSEGV, Segmentation fault.
> 0x00000000004f7789 in dinput_is_pressed (di=0x4f6f110, binds=0x0, port=2, id=7)
>     at input/drivers/dinput.c:282
> 282     input/drivers/dinput.c: No such file or directory.
> (gdb) bt
> # 0  0x00000000004f7789 in dinput_is_pressed (di=0x4f6f110, binds=0x0, port=2, id=7)
> 
> ```
> at input/drivers/dinput.c:282
> ```
> # 1  0x00000000004f7e4e in dinput_input_state (data=0x4f6f110,
> 
> ```
> binds=0x96de80 <libretro_input_binds>, port=2, device=1, idx=0, id=7)
> at input/drivers/dinput.c:489
> ```
> # 2  0x000000000042a74e in input_state (port=2, device=1, idx=0, id=7) at input/input_driver.c:464
> # 3  0x0000000000402443 in core_input_state_poll (port=2, device=1, idx=0, id=7) at core_impl.c:73
> # 4  0x000000001224472a in inputGetKeys_default ()
> 
>    from F:\Blue\Emulation\Emulators\RetroArch\cores\glupen64_libretro.dll
> # 5  0x0000000012244dc4 in egcvip_get_input ()
> 
>    from F:\Blue\Emulation\Emulators\RetroArch\cores\glupen64_libretro.dll
> # 6  0x0000000012205315 in read_controller ()
> 
>    from F:\Blue\Emulation\Emulators\RetroArch\cores\glupen64_libretro.dll
> # 7  0x0000000012205b8d in update_pif_read ()
> 
>    from F:\Blue\Emulation\Emulators\RetroArch\cores\glupen64_libretro.dll
> # 8  0x0000000012205f25 in write_si_regs ()
> 
>    from F:\Blue\Emulation\Emulators\RetroArch\cores\glupen64_libretro.dll
> # 9  0x0000000010678b7a in ?? ()
> 
> Backtrace stopped: previous frame inner to this frame (corrupt stack?)


