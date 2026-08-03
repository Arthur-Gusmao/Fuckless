## wayidle

A Wayland idle timeout tool for scripts.

wayidle waits until the compositor reports being idle for N seconds, then runs a command, or exits if none is given.

It is a small tool in the same tradition as the rest of this wiki.

### A timer, not a daemon

wayidle is smaller than an idle daemon: it waits, runs one command, and ends.

It is designed to be used from shell scripts:

```
wayidle -t 300 waylock
```

### One option set

A seat, a timeout, and an optional command.

There is no config file and nothing to learn.

### The minimal idle tool

For users who want idle handling to live in their scripts rather than in a daemon, wayidle is the honest answer.

It does one wait and one run.
