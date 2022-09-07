# RISCOSStuff
This is a place to share small programs I write.  You know those that do one or two simple things.  Some toys, some utilities, whatever else I whip up out of need or want.

These will from here on out be little useless and useful BASIC and Assembly Language programs.  They will be put inside of RISC OS ARCFS archives for distribution to preserve the filetypes.

All BASIC Programs will be in BBC BASIC V.  All Assembly Programs will have there source in BASIC using the builtin BBC BASIC assembler (simplifies the issue of what assembler to use).

Nothing will be allocated, I am an American, and we are not known for allocating applications, modules or similar.  This is the way it has always been, no reason to change now.

## Without WIMP:

It is interesting when you realize some things.  One thing I recently realized is that the programs I enjoy the most in RISC OS are those that do not use the WIMP at all.   I have began to think about this for other Operating Systems I like as well, and it is that all my most liked and used are those that do not take advantage of a Windowing System.

This goes for all kinds of programs, including some that by nature use a mouse (like Graphical Web Browsers or Paint Programs), it is the full screen graphical programs, and other command line driven software that holds me on any OS.

Thanks to my love of RISC OS I have realized what other Operating Systems I really still enjoy, including some that have had minimal use as late do to falling for the it's outdated wrong mindset.  These OS's are the kinds of OS that will drive us forward to long term computing.

### Some of the Other Operating Systems I like include:

Some with GUI as well, though different GUI's than the mainstream RISC OS or X11 WM's.

* RT-11
* Apple DOS 3.3
* ProDOS
* CP/M 86
* CP/M 68K
* DOS/65
* Lunix & LNG
* KERNAL + BASIC 2.0, 3.5, and 7.0 and CBM-DOS (Commodore 8-bit computers).
* Atari TOS.
* DR-DOS Most versions (even with GEM).
* MS-DOS 3.3 through 5.x, and 7.1 (without the GUI system).
* FreeDOS (even with OpenGEM / FreeGEM).
* RISC OS (especially without the WIMP).

Of these those that are still practicle for modern application as a primary OS are:
* DR-DOS
* MS-DOS
* FreeDOS
* Atari TOS.
* RISC OS (without WIMP).

Of the considered OS's some are still useful for many things, though not quite up to primary OS:
* KERNAL + BASIC + CBM-DOS.
* ProDOS.
* RT-11.

I put this information in the RISC OS repository so that people will understand the changes being made in other areas, as even RISC OS is going to be changing direction on this area (going more CLI oriented usage).  thinking about even building a complete RISC OS 5.27 ROM image without the WIMP or modules that require the WIMP, and an accompanning SD-Card image for the RPi.

Also I am likely to start writing alternate shells and emulators that run on RISC OS without the WIMP for using the other systems.  This also as it happens gives me a bit of an out on the one trouble in YASDOE, as dropping the Window Maanager from YASDOE will bring the size well under 128KB (two 64KB pages of the MMU).

**Time to have more fun, and help prove that the Windowing System is not needed, and CLI filemanagement, process management, and related is faster and easier than doing Window Management and WIMP paradigm.**  Do note that nothing related to Unix in on my list, that is not a very user friendly system.

Now the biggest question comes in future CPU usage for long term.

Mostly the CPU is at question.  The x86 died in the mid 1990's, when a new archetecture built around a RISC like core was created with HW emulation of the old ISA.  680x0 has been around for over 43 years and still going though not as strong.  ARM is only 39 years old (1985), and we are waiting to see if it continues or gets forgotten in favor of AARCH64.  The 6502, 65C02, 65C816S, and compatible CPUs have been going strong for the last 47 years and continues to be strong, widely used in new designs, and widely manufactured.

Then we ask how long do these CPUs last in regular usage, both in desktop computers and in embeded devices.

The 6502 has many examples of devices over 40 years old still working.  With that it is almost never the CPU that has failed, almost always something else.  This is a good sign for the 6502.  The 65C02 is thus far doing just as well, as is the 65C18 so far.  All three of these even in the cases of being overclocked for decades of continous use.

The ARMv2 and ARMv3 have very good track records in terms of long term usage thus far.  They are still only 35 years old and 31 years old respecitively, though it looks thus far as if they will keep up with the 65xxx series.

The others (680x0, z80, and x86) have high failure rates in normal usage conditions, with more than 0.1% in the first 10 years of use, more than 2% over 20 years, etc.  The failure rates go up with newer generations of these CPU's, with new failure rates of over 1% in the first decade of usage for most since 1998 to present.  For extreme long term computing we need much lower failure rates than that during normal operation.

The best canidates for sticking to for CPU's are the ARMv2/3 and 65xxx, so long as both remain widely available in ASIC.  I wonder if anyone has yet produced the fabled 65832 32-bit 65xxx CPU, that could get us moving forward well.  So as always we look ARM and we look 65xxx series.

There has never been video output HW that is as reliable as the CPU, though the VIC-IIe does a pretty good job of surviving so far, with fairly low failure rates.  No one can realy speak about the VIC-III, as there are too few in existance to really know.  I would propose a VIC-IV design that incorperates all of the features of the VIC-III, adds higher resolution support, more sprites, layers (four at least), and all the features of the 2gs VDG.  I would propose this be implemented with as low of an energy density as possible, and with feature sizes (lambda) no smaller than 0.5 micron (500nanometer).
