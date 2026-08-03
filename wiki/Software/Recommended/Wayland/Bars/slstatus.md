## slstatus

The suckless status monitor.

slstatus gathers system information and writes it as a status line, ready for a bar.

It is the same program that dwm users have used for years, and it feeds dwl just as easily.

### The dwm status, for dwl

Run it under dwl and the status appears on the bar:

```
dwl -s 'slstatus'
```

The `-s` flag makes slstatus print to stdout, which dwl reads.

### Suckless by design

slstatus is configured by editing a header and recompiling, in the honest suckless tradition.

Every module is a small function; you keep only the ones you want.

### Minimal C

CPU, memory, battery, volume, date — all in a tiny C program with no daemon and no scripting engine.

It is the most minimal status for a dwl desktop.
