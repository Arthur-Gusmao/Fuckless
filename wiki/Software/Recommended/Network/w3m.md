## w3m

A text-based web browser and pager, written in C.

w3m renders HTML in the terminal, with tables, forms, and inline images in terminals that support them.

### Browsing without a GUI

```
w3m https://example.com
w3m -dump https://example.com
```

w3m shows pages as text, navigated with keys. No window, no GPU, no browser engine.

### A browser and a pager

w3m also works as a pager for HTML input:

```
cat page.html | w3m -T text/html
```

It typesets HTML to text, which makes it a scriptable way to read the web.

### The text-mode browser

w3m is C, portable, and actively maintained in the Debian fork.

It is the browser for machines without a display, and for people who prefer reading over rendering.

### Pairs with curl

curl fetches, w3m renders:

```
curl -s URL | w3m -dump
```

Text stays text, and the web becomes just another pipe.
