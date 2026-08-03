## keyd

A keyboard remapping daemon.

keyd intercepts events at the kernel level and remaps them before the compositor ever sees them.

### Display-server-independent

keyd works through evdev and uinput, so it does not care about X11 or Wayland.

Your CapsLock-to-Escape mapping works in the compositor, the TTY, and everywhere else.

### Layers

keyd supports layers, letting one key switch the whole mapping.

This is the feature that replaces a hundred compositor-specific bindings with one config.

### A small daemon

A single daemon with one config file.

It is the minimal answer to remapping keys once, for every program.
