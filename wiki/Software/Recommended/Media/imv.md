## imv

An image viewer for Wayland and X11 written in C.

imv displays one image after another, keyboard-first, with no file browser and no panel. It is the sxiv philosophy brought to Wayland.

### View, nothing else

imv opens a directory or a list of files and steps through them.

Zoom, pan, rotate, and fit are all keybinds. There is no image organizer, no editor, no tagging, and no settings dialog.

### Native Wayland

imv renders directly on the Wayland compositor. No XWayland for Wayland sessions.

The X11 backend is optional at build time; on this wiki's desktops it is not built at all.

### From the sourcehut tradition

Written in C by exec64, with the image decoding left to standard libraries and the interface left to a config file.

Small, hackable, and portable to every Unix.
