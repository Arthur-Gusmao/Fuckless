## BearSSL

A small, correct TLS library written in C.

BearSSL implements SSL/TLS (RFC 5246) in C, designed to be secure by default, portable, and small enough for embedded systems.

### Correct and secure by default

Insecure protocol versions and algorithm choices are not supported by design.

Cryptographic implementations are constant-time by default, and MD5 is deliberately excluded.

### Small footprint

A minimal server fits in about 20 kilobytes of compiled code and 25 kilobytes of RAM.

The static linking model pulls in only the algorithms actually used, with no dynamic allocation anywhere.

### Highly portable

No malloc, no OS dependencies beyond a few string functions.

BearSSL runs on big systems and bootstrap code alike, and its code is as clean and well documented as any TLS library.

### A building block

BearSSL is not an application but a foundation.

It is the base for libtls-bearssl and for many minimal systems, including oasis.
