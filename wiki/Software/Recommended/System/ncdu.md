## ncdu

A disk usage analyzer with a text interface.

ncdu scans a directory tree and shows the biggest users of space, sorted, in a terminal UI.

### Find what eats the disk

The scan runs once; everything after is instant.

Directories collapse and expand, and the size of every entry is one keypress away. No indexing daemon, no GUI.

### A terminal tool

ncdu renders in the terminal with ncurses, so it works over SSH and on machines without a display.

It is the du with eyes, for people who live in a shell.

### Export and pipe

ncdu can write its scan to a file and read it back, so you can analyze a machine without scanning it again.

It composes the way a Unix tool should.

### Small C

ncdu is written in C, portable, and built by a single maintainer for decades.

A tool that does one thing, kept simple for a long time, belongs on this wiki.
