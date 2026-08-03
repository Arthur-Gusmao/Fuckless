## Mere

A lightweight Linux distribution built around musl libc and s6.

Mere is a minimal, understandable system where packages are immutable and upgrades are atomic.

### A package manager in Zig

The `mere` package manager is written in Zig, with a content-addressed immutable store.

### Plain directories and symlinks

No heavy abstractions: multiple versions coexist using plain directories, symlinks, and user namespaces.

### s6 for supervision

s6 handles system initialization and process supervision, no systemd.

### busybox and LLVM

busybox provides the core utilities and LLVM/Clang is the toolchain.

A modern, well-engineered take on the minimal distribution.
