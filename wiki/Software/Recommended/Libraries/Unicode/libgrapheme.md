## libgrapheme

An extremely simple freestanding C99 library for Unicode string handling.

libgrapheme provides grapheme cluster, word, sentence, and line-break segmentation, plus case detection and conversion, on UTF-8 strings.

### Unicode, done small

Segmentation follows the Unicode standard exactly, without the weight of ICU or libunistring.

The lookup tables are generated from the Unicode data and heavily compressed.

### Freestanding

The library does not depend on the C standard library at runtime.

That makes it suitable even for bare-metal applications.

### Suckless origin

Written by Laslo Hunhold, hosted on the suckless infrastructure, and licensed under ISC.

A POSIX Makefile and a C99 compiler are all that is needed to build it.

### Faster and smaller

Smaller and faster than the established Unicode libraries, with tens of thousands of conformance tests.

Unicode handling without the bloat.
