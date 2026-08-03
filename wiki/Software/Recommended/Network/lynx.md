## lynx

The oldest web browser still maintained, running in the terminal.

lynx renders pages as text with keyboard navigation, and has done so since 1992.

### The text browser

```
lynx https://example.com
lynx -dump https://example.com
```

lynx follows links, fills forms, and reads pages as pure text. There is no JavaScript engine and no graphical window.

### A terminal staple

lynx is preinstalled on many systems and works over SSH and on headless machines.

For reading documentation, man pages online, and plain web content, nothing is more universal.

### The dump mode

```
lynx -dump -nolist URL | head
```

`-dump` typesets a page to stdout, which makes lynx scriptable and pipeable like any text tool.

### Written in C

lynx is C, portable, and maintained by a small team for decades.

It is the browser for the text-first, resource-careful philosophy of this wiki.
