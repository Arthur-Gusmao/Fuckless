## musl

A minimal libc for Linux, built to be correct and small.

musl provides a C standard library and POSIX layer, statically linked-friendly, with a clean and well-documented source tree.

### A small libc

musl is designed around simplicity and correctness rather than maximum compatibility with historical behavior.

Its implementations are straightforward and its dependencies minimal, making binaries small and predictable.

### Static linking that works

musl supports static linking without the bloat and breakage common with other libcs.

A single static binary is self-contained and portable across systems with the same kernel.

### Clean implementation

The source is readable, well structured, and organized by function.

This makes musl a good base for building your own system, which is why minimal distributions adopt it.

### No GNU baggage

No glibc bloat, no legacy compatibility layers piled on top.

Just the C library your program asked for.
