## LibreSSL

A fork of OpenSSL that aims to be simpler, cleaner, and safer.

LibreSSL is the OpenBSD project's answer to OpenSSL, forked in 2014 after years of accumulated code quality problems.

### A fork with a purpose

The OpenBSD team removed about 90,000 lines of code during the fork.

Dead platforms, obsolete features, and the heartbeat code behind Heartbleed were cut. What remains is a modernized TLS and crypto stack.

### Part of the OpenBSD way

Primary development happens inside the OpenBSD tree, with the usual care for security and simplicity.

A portable version is released regularly for Linux and other systems.

### libtls included

Alongside libcrypto and libssl, LibreSSL ships libtls, a new, simpler TLS API.

libtls makes writing secure applications much harder to get wrong.

### Minimal by default

No new features, ciphers, or APIs without a solid reason.

The project's goals are simplicity, security, and sanity.
