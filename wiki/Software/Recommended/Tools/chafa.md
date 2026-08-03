## chafa

A terminal image renderer: images as text, in the terminal.

chafa converts any image into ANSI, sixel, or kitty graphics, so you can view images without a GUI viewer or a display server.

### The image-to-text bridge

```
chafa photo.png
chafa --format=symbols --colors=16 image.jpg
```

The image becomes text cells, colors, and unicode blocks, right in your terminal.

### No GUI, no server

chafa needs no display, no Wayland, and no X.

It is the tool for headless machines, SSH sessions, and any terminal that speaks color.

### Composable like any text tool

chafa reads from stdin and writes to stdout:

```
curl -s URL | chafa
```

Put it in a shell pipeline and images become part of your terminal workflow.

### Written in C

A single small C program, with the decoding left to standard image libraries and the rendering left to your terminal.
