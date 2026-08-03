## neomutt

A terminal email client, forked from Mutt, that stays textual and scriptable.

neomutt reads and writes mail as text. The interface is a terminal UI; the storage is Maildir or mbox files on your disk.

### Email as files

Messages are plain text files in a folder you own. No proprietary store, no cloud, no lock-in.

Your whole mailbox is a directory tree readable by `grep`, `awk`, and your backup tool.

### The Mutt philosophy, maintained

Mutt's design was always Unix: configure with a plain file, script everything, run in a terminal.

neomutt continues that without turning into a groupware product. Features are added, but the core stays small and the config stays text.

### Composability

Fetch and send mail with the tools of your choice: mbsync, msmtp, notmuch, or a shell loop.

neomutt does not force a server stack on you. It renders, navigates, and edits, and lets the surrounding Unix tools do the rest.

### Scriptable

Every action is bound to a key and available from the command line.

The client is hackable the way the wiki likes: if the behavior is not to your taste, you change a binding, not a setting dialog.
