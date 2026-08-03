## howl

A neuswc-based compositor controlled by an external client program.

howl splits the compositor from its controller.

The compositor itself stays tiny: it renders and manages windows. A separate client program drives it, which keeps the compositor simple and makes it scriptable from outside.

### Separating mechanism from control

Most compositors glue input handling, layout policy, and rendering into one monolithic process.

howl instead exposes control to a client program. The result is a compositor you can inspect and drive, rather than a black box you configure with great effort.

### Composability

Because control happens through a program, howl composes with the Unix philosophy.

External tools can talk to it, and users can write their own controller without forking the compositor and carrying a patch set forever.
