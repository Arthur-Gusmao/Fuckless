## st

The suckless terminal emulator, probably the most minimalist terminal on this list.

st describes itself as "a simple terminal emulator for X which sucks less".

It was written in direct response to the complexity of mainstream terminals such as xterm, whose decades of historical baggage have made it an enormous and difficult program.

Terminal emulation does not need to be that complex, and st is the proof.

### Small and auditable

st is written in C around a few thousand lines.

That is small enough for a single person to read, understand, and modify the entire terminal. The codebase is the documentation.

### Configuration is source code

st has no settings menu and no configuration language to learn.

All options live in a single `config.h` header, and customization means editing a header and recompiling.

This sounds intimidating to newcomers, but it is the honest version of what every terminal does behind the scenes.

### A base, not a product

Rather than trying to please everyone with built-in features, st ships a clean core.

The community extends it through patches: scrollback, transparency, ligatures, clipboard utilities, and dozens of other options are one diff away.

You end up with exactly the terminal you want, and nothing you do not.

### Speed

With a minimal feature set and no framework overhead, st starts instantly and responds immediately.

There is little between the keystroke and the screen.
