## cproc

A C11 compiler based on QBE.

cproc is a mostly-complete C11 compiler that uses qbe as its backend, by Michael Forney.

### A small compiler

cproc implements most of the C11 language, plus some C23 features and GNU extensions.

The frontend is written in C and is small enough to be understood as a whole.

### Self-hosting

cproc can compile itself, mcpp, gcc, and binutils.

Being able to build real software is the test that matters.

### Part of the oasis stack

cproc is the C compiler used in oasis, where it compiles the entire system.

It is also used as a compiler for other small projects that value simplicity.

### A complete toolchain piece

With qbe as its backend, cproc fills the same role as gcc or clang, but in a fraction of the code.

The compiler of the minimal ecosystem.
