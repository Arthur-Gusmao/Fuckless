## daemontools

The original process-supervision suite, by djb.

daemontools supervises daemons: it starts them, restarts them when they crash, and keeps their output in logs.

### The service directory

Each service is a directory containing a `run` program and optional `log` and `down` files.

Supervision is a file layout, which makes services trivial to add and remove.

### The idea everything else copies

`s6`, `runit`, and most modern supervisors are descendants of daemontools.

Understanding daemontools means understanding the mental model behind all of them.

### Two small programs

`supervise` watches one service; `svscan` watches a directory of services.

That is the whole design: a supervisor for each service, a scanner for the set.

### Written in C, built by djb

Small, portable, and battle-tested since the 1990s.

It is the ancestor this wiki's other supervision tools trace their design to.
