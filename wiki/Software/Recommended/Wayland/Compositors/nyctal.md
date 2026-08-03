## nyctal

A tiny Wayland compositor implemented in Go.

nyctal is among the smallest compositors around.

Instead of building on a heavyweight compositor library, it implements just enough of the Wayland protocol to manage windows, keeping the entire program small enough to be read in one sitting.

### Small enough to read

Where most compositors pull in a rendering stack and a library of protocol extensions, nyctal stays close to the wire protocol.

That keeps the codebase understandable and the dependency list short. There is less between the user and the protocol.

### Go, not C

nyctal is written in Go, a deliberate choice that trades a few platform quirks for safety and readability.

A garbage-collected compositor is unusual, and it works because nyctal's scope is small enough that the runtime cost is irrelevant.

### The minimal answer

nyctal is a demonstration that Wayland compositing does not require a vast framework.

A compositor is a program that listens on a socket and draws buffers. nyctal reminds us that this can be expressed in very little code.
