## sinit

The suckless init.

sinit is a minimal init written by the suckless project, designed to be simple enough to read in one sitting.

### Tiny by design

```
#include ...
int main(void) {
    ...
}
```

sinit is a single C file of a few hundred lines. There are no runlevels, no D-Bus, no network-manager integration.

### One job

sinit runs the init script, reaps orphans, and respawns the processes it is told to.

It does not supervise services or parse declarative configs. That work belongs to separate tools like runit or s6.

### Configurable by editing the source

Like the rest of suckless, configuration happens by editing `config.h` and rebuilding.

There is no config language to learn, and no hidden behavior.

### The suckless init

For a wiki built on suckless values, sinit is the natural base layer.

It is init reduced to its essential job, which is exactly what this wiki looks for.
