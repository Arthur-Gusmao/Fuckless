## newsboat

A terminal RSS/Atom reader that stays out of your way.

newsboat downloads feeds and presents them as a text interface. Every action is a keypress, and everything is configurable from a file.

### Text is the interface

Articles are text, feeds are text, and the list is text.

There is no browser engine, no tracking, no recommendation feed. You read what you subscribed to, in order, on your own schedule.

### The sfeed complement

Where sfeed is the Unix adapter (feeds to text, pipeable), newsboat is the interactive reader.

It fetches with libcurl, stores state in plain files, and exports to stdout so it still composes with scripts.

### A config file and keybindings

The configuration is a plain text file, and every key is remappable.

If a default annoys you, you change it in a line. Nothing requires a plugin system or a daemon.

### Minimal and hackable

newsboat is written in C++ with a small core, is stable after years of development, and runs on every Unix.

It is the reader for people who treat RSS as a protocol, not a feed of engagement.
