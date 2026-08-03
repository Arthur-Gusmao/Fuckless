## wlogout

A Wayland-based logout menu.

wlogout presents a small grid of buttons for logging out, restarting, or powering off.

### A menu, not a session manager

wlogout only displays the menu and runs the commands you associate with each button.

Session handling is your responsibility.

### Layer-shell native

The menu is drawn natively over the compositor using the layer-shell protocol.

No XWayland and no desktop-environment dependencies.

### Small C

A tiny program that turns a keybinding into a logout screen.

It is the minimal companion to a lock screen.
