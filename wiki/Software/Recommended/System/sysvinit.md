## sysvinit

The classic Unix init system, written in C.

sysvinit is the traditional PID 1: it boots the system, runs the runlevels, and reaps orphaned processes.

### The original init

```
/sbin/init
```

init is the first process the kernel starts. It reads `/etc/inittab`, runs the boot scripts, and stays as the ancestor of everything.

### A small program

sysvinit is a few thousand lines of C.

It does not supervise services, run a bus, or manage sockets. It starts the scripts and gets out of the way.

### Runlevels

Runlevels are the old Unix model: `0` halts, `6` reboots, `S` single-user.

Simple, predictable, and understood by every Unix user since the 1980s.

### The Unix baseline

sysvinit is the thing other init systems replace, and the thing against which they are measured.

It belongs here as the reference for what init can be when it stays small.
