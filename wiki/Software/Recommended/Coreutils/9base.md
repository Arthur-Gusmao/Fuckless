## 9base

Ports of Plan 9 command line tools to Unix.

9base is a minimal subset of the Plan 9 userland, ported to Unix by Anselm Garbe.

### Plan 9 utilities

It provides the classic Plan 9 tools that are missing from standard Unix: `rc`, `mk`, `sam`, `cat`, `sed`, and dozens more.

### Minimal subset

Unlike full plan9port, 9base keeps only the command line utilities, without the X11 drawing tools.

### Small and self-contained

Each tool is ported as-is and links only against libc.

It is the honest way to taste Plan 9's userland on a regular Unix system.
