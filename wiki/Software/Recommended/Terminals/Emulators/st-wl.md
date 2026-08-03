## st-wl

A fork of st for Wayland.

st-wl is a native Wayland port of the suckless terminal.

Where st talks to X11, st-wl talks to the Wayland compositor directly, keeping the same core philosophy: a small, focused terminal written in C.

### The same st

st-wl preserves what makes st valuable.

The codebase remains small and readable, configuration stays in `config.h`, and the workflow of edit, compile, and run is unchanged.

For users of Wayland who want the st experience without an X11 dependency, st-wl is the natural answer.

### A native client

Unlike running st through XWayland, st-wl is a proper Wayland client.

It uses Wayland's protocols and window management directly, staying in sync with the ecosystem it runs in rather than emulating a legacy display server.

### Minimalism preserved

Just like st, st-wl does one thing well.

It renders a terminal and gets out of the way, with no tabs, no status bars, and no settings menu that pretends to be a feature.
