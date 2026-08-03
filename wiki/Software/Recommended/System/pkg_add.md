## pkg_add

The OpenBSD package manager.

pkg_add installs and manages binary packages on OpenBSD, following the project's careful approach to the whole system.

### The OpenBSD way

```
pkg_add firefox
pkg_delete firefox
pkg_info
```

pkg_add is part of the base system, small and integrated with OpenBSD's strict, audited design.

### Software as signed sets

OpenBSD signs its packages; the tool verifies the signature at install.

The model is: packages are sets of files, checked, then placed. No daemon, no hidden service.

### One command per task

Add, delete, and query are separate small programs (`pkg_add`, `pkg_delete`, `pkg_info`).

Each does one thing, following the Unix habit the project itself is built on.

### From the dragons

OpenBSD is the OS this wiki recommends for its care and correctness.

pkg_add is that same philosophy applied to installing software: deliberate, simple, and secure.
