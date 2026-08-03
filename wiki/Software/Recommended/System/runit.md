## runit

A Unix init scheme with service supervision.

runit starts, supervises, and restarts daemons. It is small, predictable, and survives crashes of services and of the machine itself.

### Services are directories

Each service is a directory with a `run` script that execs the daemon.

There is no declarative service language to learn: a service is an executable file, plus optional log and finish scripts.

### The process supervisor

runit keeps services running: if one dies, it restarts it.

The log is a separate service, so a crashing logger never takes the daemon down with it.

### Small and fast

runit is tiny compared to systemd.

It fits the philosophy of this wiki: one task, a clear model, and no hidden machinery between boot and your processes.

### From the daemontools tradition

runit inherits the daemontools idea of process supervision, written to be simpler to build and more portable.

The whole scheme is a handful of small binaries: `runsv`, `runsvdir`, `sv`.
