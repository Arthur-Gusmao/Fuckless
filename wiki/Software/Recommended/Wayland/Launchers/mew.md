## mew

A dynamic menu for Wayland, an accurate port of dmenu.

mew displays a list of choices, filters it as you type, and prints the selection to stdout.

It is a hard fork of emenu, kept for maintainership and tidiness.

### dmenu, faithfully

mew is a full clone of dmenu, not a menu that merely looks like one.

Keybindings, behavior, and output match the original. If you know dmenu, you know mew.

### Configuration is source code

Like dmenu, mew is configured by editing a header and recompiling.

No configuration language, no settings daemon, nothing to learn twice.

### Small C

mew is written in C99 and stays small.

Next to menu libraries like bemenu, which ship a whole client-server framework, mew is the honest size for the job.

### Native Wayland

mew runs on the `zwlr-layer-shell` protocol, with no XWayland.

It works on every compositor recommended in this wiki.
