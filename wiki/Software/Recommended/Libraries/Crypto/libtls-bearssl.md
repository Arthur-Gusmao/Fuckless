## libtls-bearssl

The libtls API implemented on top of BearSSL.

libtls-bearssl brings the simple libtls interface, from LibreSSL, to the small and clean BearSSL engine, by Michael Forney.

### The best of both worlds

BearSSL is small and secure but not easy to use directly: trust anchors, SNI, and non-blocking I/O involve real work.

libtls is easy to use but tied to LibreSSL.

libtls-bearssl implements the libtls API on top of BearSSL, giving both.

### A simple, consistent API

The libtls interface is designed to be secure by default and well documented.

Common cases need only a few calls, with configuration kept out of the way.

### Nearly full libtls

Implements most of the libtls API, version 4.3.0, minus features BearSSL cannot support, like OCSP stapling and CRLs.

The regress tests from LibreSSL run against it, adapted for BearSSL.

### Written by Michael Forney

The same author as cproc, samurai, and oasis, with the same values: C, simplicity, and portability.

A small piece of the minimal system stack.
