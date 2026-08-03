## OpenRC

A dependency-based init system, written in C and shell.

OpenRC starts and stops services in order, with dependency checking, without the size of systemd.

### Init made understandable

OpenRC reads scripts in `/etc/init.d` and decides what starts when, based on declared dependencies.

The whole system is plain scripts and a small C binary. There is no binary state database to corrupt.

### Shell-native

Service scripts are shell scripts with functions like `start`, `stop`, and `status`.

Anyone can read them, and anyone can write a new service. It is init for people who trust their shell.

### Composable with any init

OpenRC replaces the service manager while letting the actual PID-1 stay whatever it is.

That modularity is the opposite of the everything-in-one-unit approach.

### From the Alpine and Gentoo worlds

OpenRC is what minimal distros use when they want control and transparency.

It matches this wiki's taste: dependencies, but no machinery you cannot read.
