## pass

A password manager built from gpg, git, and a shell script.

pass stores each password in a separate gpg-encrypted file, organized as plain directories. There is no daemon, no database, no lock file.

### Purely Unix

The store is a directory tree. Each secret is one file. Copy, move, search, and version them with the tools you already know.

Your whole password database is a folder of files you could read with cat if they were not encrypted.

### A few shell functions

pass is one POSIX shell script with a small set of commands: `pass insert`, `pass show`, `pass generate`, `pass rm`.

Each one wraps gpg for encryption and git for history. There is no proprietary format to lock you in.

### The password database as code

Because the store is git, you get history, branching, and offline sync by pushing a bare repo.

Changes are commits. Every password change is a diff you can review. This is version control for your secrets, for free.

### Composable by design

pass prints to stdout, so it composes with dmenu and clipboard tools:

```
pass show site | head -n1 | wl-copy
```

The script is short enough to read, and the gpg and git underneath are tools you already trust.
