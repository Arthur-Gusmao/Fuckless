## libinput

The input stack for Wayland compositors and display servers.

libinput handles input device detection, event processing, and abstraction, so a compositor does not reinvent input handling.

### One input stack

libinput provides device detection, event handling, and abstraction to minimize the amount of custom input code a compositor needs.

Touchpad gestures, pointer acceleration, and touch scaling are all handled by the library.

### Not for applications

libinput is not used directly by applications.

Think of it as a device driver: the Wayland compositor uses it, and clients never know it is there.

### The Wayland standard

Almost every Wayland compositor, from the minimal to the full-featured, uses libinput.

Replacing the X input drivers with one library keeps the input layer uniform.

### A fork without udev

Michael Forney maintains a fork of libinput for his compositors that drops the libudev dependency.

The core of the library remains the same, with a smaller footprint for minimal systems.
