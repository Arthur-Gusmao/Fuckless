## sfeed

RSS and Atom feeds as text.

sfeed parses feeds from stdin and writes them as a TAB-separated file, ready for `awk`, `cut`, and `grep`.

### The Unix adapter

Instead of a monolithic reader, sfeed is a set of small tools: parse, update, format, and read.

The parser is network-protocol-agnostic; fetching is left to `curl` or anything else. Feeds become plain text you already know how to process.

### A shell script as config

The configuration is a shell script that `sfeed_update` sources.

There is no declarative config language to learn, only functions and variables in `sh`.

### From the suckless community

Written in C99 by Hiltjo Posthuma, with nothing beyond libc required.

Portable to nearly every Unix, tested across many architectures and libcs.
