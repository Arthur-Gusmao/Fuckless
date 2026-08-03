## wl-clipboard

The clipboard and primary-selection tools for Wayland.

wl-clipboard provides two commands, `wl-copy` and `wl-paste`, which read and write the Wayland clipboard.

It is the direct replacement for the X11 `xclip` and `xsel`.

### Two commands, one job

`wl-copy` copies text or files to the clipboard. `wl-paste` reads from it.

They follow the Unix convention of reading and writing stdin and stdout, so they compose with pipes:

```
ls | wl-copy
wl-paste > file.txt
```

### Primary selection

Wayland has no global clipboard in the old sense.

wl-clipboard takes ownership of the selection and serves it, which is how selections work on a Wayland desktop.

### Written in C

Small, single-purpose, and universal.

Every compositor in this wiki supports the protocols it uses.
