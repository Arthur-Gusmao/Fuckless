## Why Xorg is harmful

Xorg is the display server at the heart of the traditional Unix desktop.

It is also a system from 1987 that free software has spent four decades patching instead of replacing.

This wiki is opinionated, and our position is that Xorg is not just old but actively harmful. Here is why.

### Born in another era

The core X protocol dates to 1987, when a display was a shared, trusted, single-user resource.

Its assumptions — one machine, one display, one user, everyone equally trusted — are wrong for a modern system. The protocol was designed for what computing was then, not what it is now.

### Huge by design

The Xorg server is hundreds of thousands of lines of code, and the surrounding stack multiplies it.

Much of that weight is the cost of supporting the client-server wire protocol, dozens of drivers, and three decades of accumulated extensions. Nothing about it can be subtracted, because everything has someone depending on it.

### No security model

This is the real harm. In X11, any client can read the keystrokes of any other client, capture the screen, and inject synthetic input events.

There is no isolation between windows. A single untrusted program can log everything you type everywhere, and the window system itself cannot stop it. The Xorg server also runs as root, widening the blast radius of every bug in it.

### The network transparency tax

X11's original selling point was network transparency: drawing over a wire protocol to a remote display.

That feature is barely used today, but everyone pays for it. Every draw call is serialized into the protocol, every image is marshalled to the server. The architecture is built for 1980s network performance and a 1980s trust model, and it cannot be changed without breaking everything.

### An endless pile of extensions

The core protocol was so limited that the industry rebuilt it out of extensions: RandR, Render, Composite, DRI, XInput2, GLX.

Each extension patches an original mistake instead of fixing it. The result is a spec that no one understands in full and a server that runs a museum of compromises.

### Maintenance mode

The free software world has effectively stopped developing Xorg.

It receives security fixes and little else. The feature work that used to go into the X server now goes into Wayland and XWayland. Xorg is a completed product from a completed era.

### There is a better way

Every compositor recommended in this wiki runs on Wayland, and none of them needs the X server.

The neulibs compositors and the wlroots compositors in this wiki show a working desktop without any of the above: no keystroke sniffing, no root daemon, no wire protocol, no 1987 assumptions.

### A pragmatic note

This wiki is not dogmatic. XWayland is still recommended for running legacy X11 applications on a Wayland desktop, and it is a separate, contained piece of software.

But as a display server in its own right, Xorg is the anti-recommendation of this wiki. It is the clearest example of the costs of keeping software alive because it is already there.
