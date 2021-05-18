# amisys
A BBS/packdisk menu-style replacement for Workbench with everything you need to be a productive member of the demoscene. Use a real Amiga with a compact flash IDE adapter for optimal awesome.

![amisys](https://github.com/cliffordcarnmo/amiga-hd-menu/blob/master/screenshot.jpg)

**Usage**

There are several ways to use amisys, here are a few:
* Write [**amisys.img**](https://www.carnmo.com/files/amisys.img) to a compact flash or SD-card with dd, win32diskimager or similar and put it in your real Amiga using an internal IDE adapter or use it in an external USB-IDE-adapter as harddrive in your Amiga emulator
* Clone the files in the **dh0** directory straight to your existing real Amiga harddrive or use it as harddrive path in your Amiga emulator

Please note that by writing [**amisys.img**](https://www.carnmo.com/files/amisys.img) to a compact flash or SD-card you get a properly configured system with two partitions (system: and data:) based on the PFS filesystem for superior stability and performance compared to FFS. **Please consider using amisys this way!**

**Included software**

* AHX 2.3d-sp3
* ASM-One 1.48
* BootX 4.42
* Cygnus Editor 4.2
* Disk Masher System 1.11
* Directory Opus 4.12cu
* Deluxe Paint 4.1
* DeliTracker 2.34 (players are located in s:deliplayers)
* Grabkick 1.21
* Killhappy
* PicCon 2.50
* PowerPacker 4.0a
* Protracker 2.3e
* Protracker 3.15
* Protracker 3.62
* SnoopDos 3.8
* StoneCracker 4.10.3
* SysInfo 3.24
* The Player 6.1a
* Titanics Cruncher 1.2
* TransADF 4.0.46
* Transdisk
* WhichAmiga 1.33
* X-Copy Professional
* ...if you are missing your fav tool, submit a pull request and I'll include it

**How to transfer files using an external PCMCIA adapter**

Amisys are configured to be able to mount a FAT32-formatted compact flash, SD-card or similar by using an external adapter located in the PCMCIA expansion port. Just insert your card in the adapter and run `mount cf0:`. The stuff behind the scenes to make this work is l/fat95, devs/compactflash.device and devs/dosdrivers/cf0. This is no rocket science but it makes it **very easy** to transfer files to and from your real Amiga using Windows, macOS or GNU/Linux. Yay.

**Troubleshooting**

If you are cloning this repo on Windows and plan to use the dh0 folder you need to set `git config --global core.autocrlf false` to disable automatic transformation of line endings. If you clone this repo using CRLF, you will not be able to use the dh0 folder. If you need to use CRLF under Windows, I suggest you [download the master archive from Github instead](https://github.com/cliffordcarnmo/amisys/archive/master.zip).
