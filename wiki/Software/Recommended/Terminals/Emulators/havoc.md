## havoc

A simple, fast and modern terminal emulator that does one thing and does it well.

havoc is a minimal terminal emulator for Wayland on Linux.

It follows the same spirit as st, but speaks the Wayland protocol natively instead of X11.

### Small and focused

havoc is written in C with few dependencies.

Its purpose is narrow: render a terminal on a Wayland compositor. Everything outside that scope is left out.

### Simple configuration

Configuration is done through a plain `havoc.cfg` file instead of a daemon or a settings database.

Fonts, colors, and the essentials are configured with a few lines of text, without a graphical preferences dialog hiding the actual options.

### Modern enough

Despite its size, havoc is not a toy.

It supports what a modern terminal needs, including 24-bit colors and full TUI support, so ncurses applications render correctly.

### Honest scope

havoc does not try to be a terminal multiplexer, an emulator for a dozen legacy terminals, or a platform for plugins.

It emulates a terminal and leaves the rest to the tools that do it well.
