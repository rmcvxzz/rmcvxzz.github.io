---
layout: post
title: Working on flOw PSP (US) decomp
---

flOw decompilation for the PSP

![flowy](https://i.ytimg.com/vi/R0UN4wFSNh8/sddefault.jpg)


So, for the past few days, i've been working on a decomp of flOw for the PSP (US rom). 


Well, like many decomps out there, i chose a Byte-for-Byte matching decomp, with the GCC 3.3.3+allegrex-2.2.2-psp-1.3.1 (woah long name) for diffing & PSP SDK 6.60 for compiling.
GCC Compiler provided by [decomp.me](https://decomp.me). (special thanks!)


Now, at the time of this post.... i *__WASN'T__* confident enough to release this code since it hasn't been cleaned, and 
i meant cleaned as in *__ALOT__* of ROM & Asset stuff that hasn't been cleared. Sadly though, the Assembly files will *__NOT__* be pushed to the
repo. Why? It's already self-explanatory. Let's take a look below.

`PS D:\flOwpsp\asm> (Get-ChildItem -Recurse -File).Count`


What's the output?


`5792`


Well, that makes sense, and it's (probably) smaller than other decomps.

Anyways, this decomp will hopefully utilize Makefile and C, and uhh
that's pretty much it! thanks and take care.
