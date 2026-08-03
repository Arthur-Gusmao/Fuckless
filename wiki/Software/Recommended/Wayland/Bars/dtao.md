## dtao

A stdin-based general-purpose bar for Wayland.

dtao draws text fed through a pipe onto a layer-shell bar, modeled after dzen2.

It is written by the author of dwl and carries the same taste.

### stdin in, bar out

dtao is fed by a script or a status loop:

```
while :; do date; sleep 1; done | dtao
```

The bar renders whatever the pipe provides. There is no config file and no daemon.

### dzen2 for Wayland

dzen2 was a venerable X11 bar built on the same idea: text in, colors out.

dtao brings that simplicity to Wayland, on the layer-shell protocol, with no XWayland anywhere.

### Small C

A single C file, using fcft for fonts and pixman for drawing.

It does one thing and leaves room to port the rest of dzen's formatting without much Wayland knowhow.
