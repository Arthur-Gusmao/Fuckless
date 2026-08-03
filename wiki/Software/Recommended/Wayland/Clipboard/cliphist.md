## cliphist

A clipboard history manager for Wayland.

cliphist stores clipboard history and lets you recall old entries, so a copied value is not lost the moment you copy the next one.

It is written in Go and stores its history in a single file.

### A passive recorder

cliphist is wired to `wl-paste` in watch mode:

```
wl-paste --watch cliphist store
```

It simply records everything that lands on the clipboard. It changes nothing about how the clipboard works.

### Recall without a GUI

Entries are listed to stdout and selected with a launcher like mew:

```
cliphist list | mew | cliphist decode | wl-copy
```

There is no separate window manager, daemon, or database. Just text in, text out.

### Minimal

History in one file, recall through pipes.

cliphist is the anti-bloat clipboard manager.
