## mpv

A media player based on MPlayer and mplayer2, built on the philosophy that a player is a program, not a product.

mpv plays video and audio with a tiny core and a scriptable interface. No store, no accounts, no telemetry, no branding.

### The player as a library with a CLI

At the heart of mpv is libmpv, a C library. The `mpv` binary is a thin interface to it.

That means the player is scriptable from Lua and controllable from the command line like any Unix program. One binary, no GUI framework required.

### Playback in a terminal

With `--vo=tct` or `--vo=caca`, mpv renders video in the terminal.

In a headless or minimal setup, mpv plays audio with no display at all.

### Config is a file

Everything is configured in `mpv.conf` and input bindings in `input.conf`: plain text, no database, no daemon.

What you write is what it does.

### Small and auditable

The binary is small relative to the GUI players, and the codebase is maintained by people who value correctness over features.

It plays the format, then gets out of the way.
