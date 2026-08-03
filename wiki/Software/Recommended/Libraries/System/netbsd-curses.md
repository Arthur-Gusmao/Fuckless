## netbsd-curses

A portable version of the NetBSD curses library, for Linux and musl.

netbsd-curses is a port of NetBSD's libcurses, brought into a portable shape by the sabotage-linux project.

### A small drop-in for ncurses

Close to a fully feature-complete replacement for ncurses, including wide-char support.

Programs that use the curses API build and run against it with minimal changes.

### Readable and hackable

NetBSD's curses source is far easier to change than ncurses, whose build process has several layers of preprocessing.

The port keeps a simple POSIX Makefile and no complicated build system.

### Much smaller

About 3.3 MB of extracted source versus 15.8 MB for ncurses.

Installed size is roughly a tenth, and the shared library is half the size, with far shorter build times.

### From the sabotage tradition

Developed and tested on sabotage-linux, a minimal musl-based distribution.

Curses without the ncurses weight.
