## mupdf

A lightweight PDF and EPUB viewer and toolkit written in C.

mupdf is a library, a viewer, and a set of command-line tools in one small package, built for speed and low memory use.

### One binary, many tools

The `mutool` command brings extraction, conversion, and inspection into the shell:

```
mutool draw -o page.png file.pdf
mutool extract file.pdf
mutool clean file.pdf out.pdf
```

Text and images come out of a document without opening a window.

### Fast by design

mupdf focuses on speed and a small footprint.

It handles large PDFs with low memory use, which is what makes it a good base for viewers like llpp.

### A clean library

The core is a small C library with a stable API.

The viewer and the tools share the same code, so nothing is duplicated.

### The engine behind other viewers

llpp is built on mupdf, and zathura can use it as a backend.

The toolkit is worth recommending on its own, even without the graphical viewer.
