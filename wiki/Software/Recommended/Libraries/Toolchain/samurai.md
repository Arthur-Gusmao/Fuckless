## samurai

A ninja-compatible build tool written in C.

samurai is an alternative implementation of the ninja build system, in a single C file.

### Ninja-compatible

samurai reads the same build files as ninja and runs the same build.

Projects that use ninja can use samurai without changes.

### One C file

The entire build tool is a single C file.

No dependencies beyond the C standard library, built with a plain Makefile.

### Fast and small

samurai is faster than ninja and much smaller.

Alpine Linux uses samurai as its primary ninja implementation, a strong endorsement of its quality.

### A component of the minimal toolchain

By Michael Forney, in the same family as cproc and qbe.

A build tool that does not need a build system to build itself.
