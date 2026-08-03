## brightnessctl

Control of screen and keyboard brightness.

brightnessctl reads and sets brightness through the kernel's backlight and leds interfaces.

### The xbacklight replacement

On X11, `xbacklight` was the standard tool.

It does not work on Wayland, so brightnessctl, which talks to the kernel directly, has become the standard on Wayland desktops.

### Device agnostic

brightnessctl lists the devices it can control and sets them by name or index.

It also handles keyboard backlight, which no X11 tool managed.

### One binary

A small C program that reads and writes sysfs files.

It composes with keybindings to show feedback while you change brightness.
