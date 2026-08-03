## Why portals are harmful

Portals are a mechanism for Wayland applications to reach the system without the compositor trusting them.

xdg-desktop-portal-wlr implements screen sharing and global shortcuts through a D-Bus daemon. The name sounds neutral. The design is not.

### A daemon in the middle

A portal is a running service that translates generic requests into compositor requests.

The compositor no longer talks to applications directly. A daemon sits in between, becoming a new layer of trust, a new moving part, and a new thing that can break, all to serve features the base protocol could handle.

### Protocol bloat on demand

Portals exist to paper over gaps in the Wayland protocol.

Screen sharing and shortcuts have no solid native path in the common compositor libraries, so the answer was not to fix the protocol but to add a daemon. Every feature becomes a new portal interface, and the desktop grows a second protocol stack.

### It drags in D-Bus

The portal design assumes D-Bus is acceptable.

D-Bus is a dependency this wiki does not want. A minimal Wayland stack should not require a message bus daemon just to share a screen.

### The neulibs answer

The neulibs ecosystem in this wiki handles this differently: no portals, no plugin runtime, no settings daemon. What you read is what runs.

When a feature needs the compositor, the compositor grows the protocol. There is no middleman, no D-Bus, and no second way to do the same thing.

