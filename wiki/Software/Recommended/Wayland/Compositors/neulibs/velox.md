## velox

A simple tiling compositor for Wayland, built on swc.

velox brings the dwm model to Wayland.

Windows are arranged in tiles automatically, and configuration is done by editing a header and recompiling. The philosophy will be familiar to anyone who used dwm.

### dwm, reborn on Wayland

velox inherits the ideas that made dwm successful: dynamic tiling, a small codebase, and configuration through source code.

Instead of a settings daemon or a configuration language, customization lives in `config.h`.

### Built on swc

velox is built on swc, the small compositor library written by michaelforney.

Rather than depending on wlroots and its ecosystem of protocol extensions, velox relies on a library small enough to audit, keeping the whole stack comprehensible.

### A whole system you can understand

From the compositor library to the compositor itself, velox is part of a stack designed to be read and modified.

For users who want to own their desktop, that is the point.
