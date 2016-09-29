# Luma3DS
*Noob-proof (N)3DS "Custom Firmware"*

THIS IS FOR 11.1 ONLY AT THE MOMENT

This is a fork of Luma3DS that spawns a thread payload of user-supplied code for RAM editing, RAM dumping, or any other purpose you might need. You need to use my thread payload with this at https://github.com/Bond697/LumaThreadN3DS

To use this fork: you should be able to simply run the batch to build and copy the arm9loaderhax.bin to your sd card.  

Caution!
If you make a really huge thread.bin, you may have to update the read size at the bottom of patches.c.  The size is currently set to 0x6800 bytes, so almost no one should have to change it.

## What it is

**Luma3DS** is a program to patch the system software of (New) Nintendo 3DS handheld consoles "on the fly", adding features (such as per-game language settings and debugging capabilities for developers) and removing restrictions enforced by Nintendo (such as the region lock).
It also allows you to run unauthorized ("homebrew") content by removing signature checks.  
To use it, you will need a console capable of running homebrew software on the ARM9 processor. We recommend [Plailect's guide](https://github.com/Plailect/Guide/wiki) for details on how to get your system ready.

---

## Compiling

First you need to clone the repository recursively with: `git clone --recursive https://github.com/AuroraWright/Luma3DS.git`  
To compile, you'll need [armips](https://github.com/Kingcom/armips) and a build of a recent commit of [makerom](https://github.com/profi200/Project_CTR) added to your PATH.  
For now, you'll also need to update your [libctru](https://github.com/smealum/ctrulib) install, building from the latest commit.  
For your convenience, here are [Windows](http://www91.zippyshare.com/v/ePGpjk9r/file.html) and [Linux](https://mega.nz/#!uQ1T1IAD!Q91O0e12LXKiaXh_YjXD3D5m8_W3FuMI-hEa6KVMRDQ) builds of armips (thanks to who compiled them!).  
Finally just run `make` and everything should work!  
You can find the compiled files in the `out` folder.

---

## Setup / Usage / Features

See https://github.com/AuroraWright/Luma3DS/wiki

---

## Credits

See https://github.com/AuroraWright/Luma3DS/wiki/Credits

---

## Licensing

This software is licensed under the terms of the GPLv3.  
You can find a copy of the license in the LICENSE.txt file.
