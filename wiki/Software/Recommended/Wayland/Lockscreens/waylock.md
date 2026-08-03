## waylock

A simple screen locker for Wayland.

waylock locks the screen and unlocks on the correct password, with none of the machinery of the X11 lockers.

It is by the author of river.

### Simpler than swaylock

waylock does not talk to PAM and does not depend on a system-wide authentication stack.

The password is stored as a hash in a config file, and waylock compares against it. The whole design is a few hundred lines.

### One job

Lock the screen, verify the password, unlock.

No fingerprint handlers, no multi-monitor panels, no features you will read about twice.

### Native Wayland

waylock draws its own lock screen over the compositor, with no XWayland.

It is the minimal locker for a minimal desktop.
