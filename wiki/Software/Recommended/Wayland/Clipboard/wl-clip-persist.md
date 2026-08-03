## wl-clip-persist

Persists the Wayland clipboard after its source closes.

On Wayland, copied data dies when the copying program exits. wl-clip-persist re-owns the selection so the data survives.

### Fixing a Wayland quirk

The clipboard is served by the copying client, not stored anywhere.

wl-clip-persist watches the selection and takes it over before the source closes, keeping the old value available.

### A background helper

It runs in the background, quietly, and does nothing you notice.

Paired with wl-clipboard and cliphist, it makes the clipboard behave like the one users remember from X11.

### Small C

A tiny single-purpose daemon.

It fixes one annoyance and nothing else.
