## doas

A minimal replacement for sudo, from OpenBSD.

doas runs a command with elevated privileges, configured by one short file. No daemon, no timeout daemon, no huge codebase.

### The configuration is the whole app

```
permit keepenv user as root
permit nopass :wheel
```

Five lines and you are done. There is no `visudo`, no editor shipped with it, and no plugin system.

### Tiny and auditable

doas is a few thousand lines of C.

The sudo codebase has more moving parts than the privilege switch it performs. doas is a fraction of that, which makes it possible to read and verify.

### OpenBSD design

doas comes from OpenBSD, the project this wiki already recommends for its care and correctness.

It keeps the Unix habit of doing one thing, done well, with as little as possible.

### Ports cleanly

The portable version builds on any Unix with make and a C compiler.

No autotools madness, no Python, no message bus.
