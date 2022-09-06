# RISCOSStuff
This is a place to share small programs I write.  You know those that do one or two simple things.  Some toys, some utilities, whatever else I whip up out of need or want.

These will from here on out be little useless and useful BASIC and Assembly Language programs.  They will be put inside of RISC OS ARCFS archives for distribution to preserve the filetypes.

All BASIC Programs will be in BBC BASIC V.  All Assembly Programs will have there source in BASIC using the builtin BBC BASIC assembler (simplifies the issue of what assembler to use).

Nothing will be allocated, I am an American, and we are not known for allocating applications, modules or similar.  This is the way it has always been, no reason to change now.

# Without WIMP:

It is interesting when you realize some things.  One thing I recently realized is that the programs I enjoy the most in RISC OS are those that do not use the WIMP at all.   I have began to think about this for other Operating Systems I like as well, and it is that all my most liked and used are those that do not take advantage of a Windowing System.

This goes for all kinds of programs, including some that by nature use a mouse (like Graphical Web Browsers or Paint Programs), it is the full screen graphical programs, and other command line driven software that holds me on any OS.

Thanks to my love of RISC OS I have realized what other Operating Systems I really still enjoy, including some that have had minimal use as late do to falling for the it's outdated wrong mindset.  These OS's are the kinds of OS that will drive us forward to long term computing.

### Some of the Other CLI Operating Systems I like include:

* RT-11
* Apple DOS 3.3
* ProDOS
* CP/M 86
* CP/M 68K
* DOS/65
* Lunix & LNG
* KERNAL + BASIC 2.0, 3.5, and 7.0 and CBM-DOS (Commodore 8-bit computers).
* DR-DOS Most versions.
* MS-DOS 3.3 through 5.x, and 7.1 (without the GUI system).
* FreeDOS.
* RISC OS.

Of these those that are still practicle for modern application as a primary OS are:
* DR-DOS
* MS-DOS
* FreeDOS
* RISC OS (without WIMP).

Of the considered OS's some are still useful for many things, though not quite up to primary OS:
* KERNAL + BASIC + CBM-DOS.
* ProDOS.
* RT-11.

I put this information in the RISC OS repository so that people will understand the changes being made in other areas, as even RISC OS is going to be changing direction on this area (going more CLI oriented usage).  thinking about even building a complete RISC OS 5.27 ROM image without the WIMP or modules that require the WIMP, and an accompanning SD-Card image for the RPi.

Also I am likely to start writing alternate shells and emulators that run on RISC OS without the WIMP for using the other systems.  This also as it happens gives me a bit of an out on the one trouble in YASDOE, as dropping the Window Maanager from YASDOE will bring the size well under 128KB (two 64KB pages of the MMU).

**Time to have more fun, and help prove that the Windowing System is not needed, and CLI filemanagement, process management, and related is faster and easier than doing Window Management and WIMP paradigm.**  Do note that nothing related to Unix in on my list, that is not a very user friendly system.
