## wev

A Wayland event debugger, the analog of xev.

wev prints the Wayland events a client receives: key presses, pointer motion, and touch input, as they happen.

### Debug your input stack

```
wev
wev --names
```

Run it, press keys, and read the protocol events on stdout. There is no GUI, no state, no config.

### A raw view of the protocol

wev shows the same events the compositor delivers, including the serials and modifiers.

That makes it the tool to verify that keybindings, grab tricks, and shortcuts work as expected.

### From the same hand as ydotool

wev is a small C program in the tradition of wtype and the Wayland debug tools.

Minimal, readable, and exactly one job.

### Pairs with wtype

Wev shows what the compositor receives; wtype sends input back.

Together they are the two ends of input debugging on Wayland.
