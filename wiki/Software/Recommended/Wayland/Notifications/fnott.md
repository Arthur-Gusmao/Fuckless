## fnott

A minimal notification daemon for Wayland.

fnott displays desktop notifications on the screen using the `zwlr-layer-shell` protocol, which the compositors in this wiki support.

### One binary, no X

fnott runs natively on Wayland with no XWayland and no desktop-environment baggage.

It renders notifications itself; it does not embed a web engine.

### Configured by a small file

fnott reads a single configuration file.

There is no GUI, no theme engine, and nothing to learn beyond a handful of options.

### From the foot author

fnott is by the author of the foot terminal, a developer whose taste matches this wiki's philosophy.

It is stable, small, and does one thing.
