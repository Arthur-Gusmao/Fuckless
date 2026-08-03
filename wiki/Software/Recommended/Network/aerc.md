## aerc

A terminal email client with a modern touch, written in Go.

aerc presents your mail in a split screen: the message list and the reader side by side, with a composer that opens when you reply.

### Client, server, and filters composed

aerc reads and writes mail, and delegates transport to the tools of your choice.

Fetch with mbsync or your own script, and let aerc handle reading, replying, and sending. Accounts are configured in a plain file.

### A TUI for fast email

The interface is keyboard-first with a vi flavor.

Panes, keybindings, and filters are configured in text files; nothing hides behind a settings dialog.

### The composer as a file

New mail opens in your `$EDITOR`. When you save and quit, aerc sends.

That makes email writing exactly as flexible as your editor, and it means scripts and signatures work as they do in vim.

### From the Go tradition

aerc is a single binary, portable, and easy to build.

It is the email client for people who want mail in the terminal without giving up modern conveniences.
