## cmus

A small, fast terminal music player for Unix.

cmus plays music from the command line with a text interface, handling large libraries without a GUI or a database server.

### The library as files

cmus scans a directory tree; the library is the files themselves.

No import step, no proprietary store, no network. Point it at your music folder and it plays.

### A TUI you control

The interface is ncurses with vi-like bindings.

Playlists, queues, and the library are all reachable from the keyboard, and every binding is changeable.

### Scriptable

cmus talks to a remote control socket:

```
cmus-remote -p
cmus-remote -q
cmus-remote -C "view now-playing"
```

Scripts and keybindings drive it, which makes it the terminal companion to a minimal desktop.

### From the terminal tradition

cmus is C, portable, and plays the formats your system has decoders for.

It is the music player for a machine that wants to play music, and nothing else on the screen.
