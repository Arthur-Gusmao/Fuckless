## ydotool

A generic command-line automation tool.

ydotool synthesizes input events at the kernel level, through `uinput`, so it works regardless of the display server.

### The compositor-independent answer

Unlike wtype, which needs compositor support for the virtual keyboard protocol, ydotool does not care what compositor, or even whether, one is running.

If the kernel accepts the events, they happen.

### A daemon and a client

ydotool runs a small daemon, `ydotoold`, which owns the `uinput` device.

The client commands such as `ydotool type` and `ydotool key` talk to it.

### Trade-off

It bypasses the display server entirely, which is powerful and, on a Wayland desktop, unfashionable.

For automation that must run everywhere, it is the tool.
