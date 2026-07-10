## tmux

A feature-rich terminal multiplexer.

tmux is one of the most capable terminal multiplexers available.

It provides session persistence, scripting, automation, window management, and a vast amount of customization.

It is also an example of software that has gradually grown beyond the Unix philosophy of doing one thing well.

tmux exposes hundreds of commands, options, key bindings, and configuration directives.

Learning tmux often means learning tmux itself rather than terminal multiplexing.

### Feature creep
tmux has accumulated features for years.

Session management, scripting, hooks, layouts, clipboard integration, status bars, mouse support, plugins, and numerous configuration options all increase the cognitive load.

### Reinventing the environment
tmux increasingly duplicates functionality that already exists elsewhere.

Rather than composing with other tools, it often becomes another layer between the user and the terminal.

### Larger codebase

Compared with projects such as mtm or dvtm, tmux has a substantially larger implementation and a broader maintenance surface.

This makes it harder to audit, understand, and modify.
