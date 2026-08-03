## neatvi

A minimal vi implementation focused on simplicity, portability, and correctness.

neatvi is not a Vim clone.

It is a modern implementation of the original vi philosophy: a small editor that does one thing well.

### The vi model, refreshed

neatvi implements the classic vi editing model with a clean, modern codebase.

Modal editing, ex commands, and the composability that made vi famous are all present, without the decades of accumulated extensions found in Vim.

### Small enough to understand

Unlike editors that grew into operating systems, neatvi stays small enough for a single developer to maintain and a curious user to read.

The whole editor is a manageable amount of C, free of external dependencies and framework baggage.

### Portable

neatvi compiles and runs on a wide range of Unix-like systems with minimal fuss.

It does not depend on a package manager, a plugin ecosystem, or a language runtime. It is a program, not a platform.

### Do one thing well

neatvi is an editor. It does not try to be a file explorer, a terminal multiplexer, or an integrated development environment.

That focus is exactly what makes it reliable and easy to reason about.
