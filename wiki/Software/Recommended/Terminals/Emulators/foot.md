## foot

A fast, lightweight, minimalistic terminal emulator for Wayland.

foot is the natural Wayland-native companion to st: small, terminal-focused, and free of the frameworks that drag on GTK and Qt terminals.

It is by the same author as fnott.

### Native Wayland

foot renders directly over the Wayland compositor.

There is no XWayland, no VTE library, and no generic toolkit dictating how a terminal should behave.

### Fast

Foot is optimized to be fast: it avoids redrawing what has not changed and uses the GPU when it helps.

It starts quickly and keeps up with the fastest text.

### Configured by a file

foot reads a single `foot.ini`.

The configuration is short and documented, and defaults are sane.

### The minimal Wayland terminal

For the same reasons this wiki recommends st on X11, it recommends foot on Wayland.

It is the terminal a minimal Wayland desktop deserves.
