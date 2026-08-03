## zathura

A minimal keyboard-driven document viewer written in C.

zathura displays PDF, PostScript, DjVu, and EPUB through plugin backends, with a config file instead of a settings dialog.

### The viewer, not the suite

zathura renders documents through poppler, mupdf, or other backends, keeping the core small.

There is no toolbar, no menu, and no mouse-first interface. Navigation is vi-style: `j`/`k` scroll, `/` searches, `r` reloads.

### Plugin backends

Each document format is a separate plugin, so the viewer only loads what a document needs.

Backends stay independent of the core, and adding a format does not bloat the program.

### Configurable by text

Keybindings and colors live in a plain config file, following the same philosophy as the rest of this wiki.

A minimal program with a text interface, out of the way until you need it.

### Works on Wayland

zathura runs as a native Wayland client through GTK, with no X11 requirement on Wayland sessions.
