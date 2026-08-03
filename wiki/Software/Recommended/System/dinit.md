## dinit

A minimal, dependency-aware init system and service supervisor.

dinit boots a system and supervises its services without systemd's scope.

### Dependencies, not magic

Services declare what they depend on, and dinit starts them in order, in parallel where possible.

A service is a small text file with a command and a list of dependencies. No binary config, no code generation.

### It does one job

dinit is an init and a process supervisor, nothing more.

It does not take over logging, mounts, or hardware; those stay with the tools designed for them.

### Small and portable

Written in C++ with minimal dependencies, used as init by Chimera Linux and available on several BSDs and Linux distributions.

It is the answer to systemd's size: a boot system you can read.
