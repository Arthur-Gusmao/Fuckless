## htop

An interactive process viewer for the terminal.

htop shows running processes with CPU, memory, and swap usage, in a color-coded screen you can navigate and act on.

### top, but interactive

```
htop
```

Scroll, search, filter, and kill processes directly from the screen. There is no GUI, no daemon, and no web dashboard.

### A terminal tool

htop renders with ncurses and works over SSH and on machines without a display.

It is the immediate answer to "what is eating my CPU" in a shell.

### Filtering and trees

Search by name, filter by user, and toggle a process tree to see parents and children.

Everything is a keypress, and the configuration is a plain file.

### Written in C

htop is C, portable, and small enough to run on minimal systems.

It replaces `top` for humans, while staying in the same resource-conscious tradition.
