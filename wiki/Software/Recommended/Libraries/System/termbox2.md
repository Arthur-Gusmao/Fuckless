## termbox2

A slim terminal I/O library for TUIs, in a single C header.

termbox2 is a minimal alternative to ncurses, with a tighter API and no dependencies beyond libc.

### A tighter API

Where ncurses grows features, termbox2 keeps the interface small.

The library handles terminal input and output; widgets and layout are left to the application, as they should be.

### Single header

Everything is in one header, `termbox2.h`.

No build system, no configuration, no library to link beyond what the compiler already does.

### Works without terminfo

termbox2 has built-in support for common terminals when no terminfo database is present.

That makes it portable to minimal systems that skip ncurses entirely.

### Successor to termbox

termbox2 keeps the simple API of the original termbox and adds stricter error handling.

The original is deprecated in its favor.
