## tig

A text-mode interface for git.

tig shows your repository in the terminal: history, diffs, branches, and staged files, navigated with keys.

### git, browsable

```
tig
tig log
tig show <commit>
tig status
```

Each view is a different angle on the same repository, without leaving the terminal.

### The command mode

At its heart tig is an interface over git commands.

Press keys to move, `!` to run arbitrary shell commands, and every action maps to the git you already know.

### In the Unix tradition

tig is a small C program with ncurses.

It renders plain text, scripts cleanly, and works over SSH and on machines with no GUI.

### Pairs with git

git handles version control; tig makes the history legible.

For a wiki built around minimal tools, tig is the readable face of the one tool everyone needs.
