## entr

A standalone file watcher.

entr runs arbitrary commands whenever the listed files change.

### Files in, command out

entr reads a list of files from standard input and executes a command when any of them change:

```
find src -name '*.c' | entr make
```

It is the missing "watch" flag for everything, without every tool shipping its own watcher.

### No config, no daemon

entr has no configuration file and no built-in file search.

It deliberately relies on `find` and friends for the list, keeping itself to the single job of reacting to events.

### Small C

A tiny C program using the kernel's file notification facility, portable across the BSDs and Linux.
