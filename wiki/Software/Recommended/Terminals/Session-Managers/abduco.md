## abduco

A session manager for terminal applications.

abduco does one thing: it allows terminal applications to detach from one terminal and reattach to another.

### One feature

abduco is not a terminal multiplexer.

It does not manage panes, layouts, or windows. It only detaches and reattaches sessions.

### A composable piece

abduco follows the Unix philosophy of solving a single problem well.

Instead of combining session management with terminal multiplexing, it leaves multiplexing to dedicated tools such as dvtm or mtm.
