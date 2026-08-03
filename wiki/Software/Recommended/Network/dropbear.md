## dropbear

A small SSH client and server built for embedded systems.

dropbear implements SSH with a fraction of OpenSSH's size: a static binary around a megabyte, no bloat, no server side-channels.

### Small enough to ship

Dropbear's server is designed for routers and embedded devices. The binary is small enough that nothing stops you from running it on anything you own.

Less code means fewer bugs, and fewer dependencies to maintain.

### Client and server in one

`dbclient` is the client, `dropbear` is the server. Both support the modern SSH ciphers and key types you already have.

It is a drop-in for the common case: log in, forward ports, run commands.

### The mosh question

dropbear replaces OpenSSH, the transport itself. mosh is not a transport: it wraps an SSH connection so it survives network changes and hides latency.

If you live on flaky mobile links, mosh is the tool for that. If you want the smallest possible SSH, dropbear is the tool for that. They solve different problems.
