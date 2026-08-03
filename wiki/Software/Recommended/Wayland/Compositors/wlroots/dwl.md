## dwl

dwm for Wayland.

dwl is a compact, hackable compositor for Wayland, based on wlroots.

It aims to fill the same space in the Wayland world that dwm fills in X11, both in philosophy and in functionality.

### The dwm model

dwl keeps everything dwm users value: dynamic tiling, tags, a master area, and keyboard-driven window management.

Windows are arranged automatically and operated from the keyboard. The mental model carries over unchanged from dwm.

### Configuration is source code

Like dwm, dwl is configured by editing `config.h` and recompiling.

There is no configuration language to learn and no settings daemon. What you want is written directly into the program you run.

### Patch culture

Optional features live outside the main codebase, as patches.

The dwl community maintains a patches repository, so the core stays lean while the ecosystem grows. You build exactly the compositor you want.

### A wlroots compositor

dwl is built on wlroots, which provides the low-level protocol and hardware handling while dwl implements the policy.

Because a Wayland compositor also takes on the role of the display server, dwl cannot be as small as dwm, but it stays as small as the job honestly allows.
