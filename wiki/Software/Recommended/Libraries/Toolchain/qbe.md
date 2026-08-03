## qbe

A small compiler backend.

qbe provides the code generation half of a compiler, written in C, in about 10,000 lines of code.

### Backend only

qbe is not a compiler. It consumes an intermediate representation and emits assembly.

Compiler frontends like cproc and Hare use it, leaving the language work to them.

### A few thousand lines

The whole backend is small enough to read in one sitting.

Clang and GCC are thousands of times larger; qbe aims to be understandable.

### Good enough code

qbe does not produce the fastest binaries on earth, but it produces good ones.

For small systems and small projects, that trade is worth it.

### The heart of a minimal toolchain

qbe powers cproc, the C11 compiler used by oasis and capable of bootstrapping itself.

A backend, not a language: one part of a coherent minimal stack.
