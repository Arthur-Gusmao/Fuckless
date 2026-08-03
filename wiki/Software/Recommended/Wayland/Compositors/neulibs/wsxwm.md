## wsxwm

A tiling compositor based on neuswc.

wsxwm comes from the creator of sxwm, the X11 tiling window manager.

It brings that same approach to Wayland: automatic tiling layouts that adapt as windows open and close, without the ceremony of a full desktop environment.

### From the sxwm lineage

sxwm earned a reputation for being a small, focused tiling window manager.

wsxwm carries that lineage forward, applying the same discipline to Wayland instead of extending an X11 codebase that was never designed for it.

### Tiling without complexity

Windows are managed automatically by layout, not by hand.

There is no tab system, no animation framework, no taskbar competing with your status bar. The compositor tiles, and the user works.

### A stack you can audit

Like the other neuswc compositors, wsxwm stands on a small, readable foundation.

The whole desktop can be understood by reading a few source files, which is exactly how it should be.
