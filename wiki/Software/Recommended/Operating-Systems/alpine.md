## Alpine

A minimal Linux built on musl and busybox.

Alpine is a security-oriented Linux that keeps the default installation tiny.

### musl and busybox

No glibc, no GNU coreutils: the base system is busybox over musl libc.

### Small by default

A base install is a few hundred megabytes, with no unnecessary services.

### Simple init

OpenRC init with plain shell scripts, no systemd machinery.

The standard minimal base for containers and small systems.
