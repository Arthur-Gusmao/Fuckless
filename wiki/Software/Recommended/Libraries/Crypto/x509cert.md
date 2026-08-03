## x509cert

A tool and library for generating X.509 certificates and certificate requests.

x509cert is Michael Forney's small C library and tool for creating X.509 certificates, built on BearSSL.

### A tool and a library

As a command, it generates certificates for local use.

As a library, it exposes the same functionality to programs that need to create certificates programmatically.

### Built on BearSSL

Uses BearSSL as its cryptographic base, keeping the dependency small and the code honest.

The natural companion to libtls-bearssl in the minimal TLS stack.

### Simple by design

X.509 is a complex standard, but the common cases are simple.

x509cert handles those cases without pulling in a large crypto framework.

### From the Michael Forney ecosystem

Written in C, released under the ISC license, and maintained with the same minimal values as the rest of his projects.
