## wtype

The xdotool replacement for Wayland.

wtype types text and sends keyboard events to the focused window.

### Why it exists

On X11, xdotool did the job of synthesizing input.

Wayland has no global event injection for security reasons, so wtype works within the compositor's input pipeline, using the `virtual-keyboard` protocol.

### Compositor support

wtype requires compositor support for the virtual keyboard protocol.

The compositors recommended in this wiki are small and focused, so check that yours enables it.

### Small C tool

One binary, one job: type the text you give it.

wtype is the honest replacement for the parts of xdotool that Wayland allows at all.
