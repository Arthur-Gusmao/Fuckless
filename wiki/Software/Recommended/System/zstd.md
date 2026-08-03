## zstd

A fast, lossless compression algorithm and command-line tool.

zstd compresses near the ratio of gzip or xz but at much higher speed, with a small decompressor that needs no library.

### Speed with real compression

zstd decompresses at gigabytes per second, which changes how compression is used.

Fast compression makes it reasonable to compress backups, logs, and package caches that gzip would slow down.

### Command-line compatible

```
zstd file
zstd -d file.zst
zstd -t file.zst
```

The tool works like gzip, and the format has a standard file suffix and headers.

### One tool, several needs

Levels trade speed for ratio, and `--long` handles big files.

The same binary covers casual compression and archive workflows without a second tool.

### Small decompressor

The decompression side is a few hundred kilobytes, easy to ship in boot images and embedded systems.

That is why it replaced zlib in many minimal projects: same job, less machine.
