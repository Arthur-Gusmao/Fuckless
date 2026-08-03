## neubar

An event-driven status bar feeder for mojito.

neubar supplies mojito with status text, replacing the usual polling shell scripts.

### Event-driven, not polled

Instead of re-running scripts every second, neubar receives updates when things change.

It listens to the neuwm IPC for workspace and mode updates, and inotify for the package count.

### Less work, same status

The system is quiet until something changes.

No busy loop, no wasted cycles, no shell-script fireworks.

### A neulibs pairing

neubar is built around the neuwm compositor's IPC.

It is the current status side of the mojito bar on a neuswc desktop.
