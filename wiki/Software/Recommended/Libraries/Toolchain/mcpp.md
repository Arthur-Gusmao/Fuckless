## mcpp

A portable C preprocessor.

mcpp is a C preprocessor written by Michael Forney, used as the preprocessor for cproc and other small compilers.

### A preprocessor, alone

mcpp does one thing: process C preprocessor directives.

It is not part of a larger compiler, so it can be used and tested in isolation.

### Portable and small

A single small program written in C, released under a permissive license.

It has been ported to the platforms where minimal toolchains are used.

### The cproc preprocessor

cproc uses mcpp for preprocessing, keeping the compiler frontend focused on parsing.

The two projects are developed together.

### Minimal toolchain component

Another piece of the coherent stack from Michael Forney, alongside qbe, cproc, and samurai.

Preprocessing without the bloat of a full compiler suite.
