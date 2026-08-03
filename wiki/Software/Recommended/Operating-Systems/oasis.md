## Oasis

A small statically-linked Linux system.

Oasis is a Linux system closer in spirit to a BSD, built entirely from small, simple components.

### sbase, ubase, sinit

musl for libc, sbase instead of coreutils, ubase instead of util-linux, and sinit with perp instead of sysvinit or systemd.

### Completely static

Every binary in the base is statically linked, including the velox display server and the netsurf browser.

### No package manager

You configure sets of files in Lua; the build system writes the resulting filesystem tree into a git repository, ready to merge into `/`.

### Extensible via pkgsrc

Software that does not fit the base goals can be installed through pkgsrc or nix, keeping the base small.

### A coherent stack

Built with samurai, cproc, BearSSL, oksh, and vis: every replacement is smaller and simpler than the mainstream one.
