## sfm

sfm (Simple File Manager) is a terminal file manager that combines a small codebase with a practical set of file management features. It is designed to be fast, keyboard-driven, and efficient for daily use without sacrificing the Unix philosophy.

Despite its name, sfm offers a rich set of features while remaining compact and easy to use. It focuses on improving productivity inside the terminal without becoming a full desktop environment or replacing standard Unix tools.

### Small implementation

sfm is a single C program with no heavy dependencies.

Its codebase stays readable and auditable, in the spirit of the projects that inspired it. Less code means fewer bugs and a smaller surface to maintain.

### Two panes, no clutter

The dual-pane interface makes comparing directories and moving files between them immediate.

A status bar shows what is going on without demanding attention, and vim-like key bindings let experienced users stay in flow.

### Observant, not polluting

sfm monitors the filesystem through the kernel's own notification mechanisms, on Linux and BSD alike.

It reacts to changes as they happen instead of polling or fighting the system, keeping resource use low while staying up to date.

### Built to be combined

sfm handles the picking and organizing, and standard Unix tools handle the rest.

It works alongside the shell and the command line rather than hiding them behind an abstraction layer.
