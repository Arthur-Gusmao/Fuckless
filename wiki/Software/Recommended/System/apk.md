## apk

The Alpine package manager: a fast, simple way to install software.

apk adds, removes, and upgrades packages with a tiny footprint and no extra moving parts beyond the package database.

### The Alpine package manager

```
apk add firefox
apk del firefox
apk upgrade
```

apk is used by Alpine Linux, the minimal system this wiki recommends. The two are the same philosophy: small, fast, and auditable.

### Fast and transactional

apk keeps a single database and resolves dependencies on the fly.

It is built to run on Alpine's musl-based systems, so it inherits that OS's care for resource use and simplicity.

### One tool for every package task

Install, remove, search, upgrade, and check are all subcommands of `apk`.

There is no separate package manager, no GUI, and no daemon to keep alive.

### Written in C

apk is a small C program, maintainable and portable to any system built the Alpine way.

It is the package manager for people who want packages without bloat.
