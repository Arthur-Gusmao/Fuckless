## greetd

A minimal login manager.

greetd starts a user session on a TTY and, when it ends, starts another. It is the smallest honest login manager.

### A manager, not a greeter

greetd only manages sessions.

The greeter itself is a separate program, chosen by the user, which makes greetd greeter-agnostic.

### Works with Wayland

greetd launches any session command, including a Wayland compositor.

It is the standard minimal way to boot into dwl, river, or a neulibs compositor without a display manager suite.

### Small C

A tiny daemon that runs one command and waits.

It is the anti-GDM.
