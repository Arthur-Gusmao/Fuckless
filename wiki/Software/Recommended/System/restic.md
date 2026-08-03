## restic

A backup program that does one thing: encrypted, deduplicated backups.

restic stores snapshots in a repository on a local disk or any remote. Each snapshot is a point-in-time copy of your files.

### Encrypted by design

Every byte is encrypted with AES-256 before leaving your machine. The server never sees plaintext.

There is no trust model that depends on the storage location; a hacked remote gives an attacker ciphertext only.

### Deduplication without a daemon

restic splits files into chunks and stores each chunk once. Restore any snapshot from any point in time with a single command.

The dedup index is local, so no server-side daemon or protocol is needed.

### The Unix way of backup

restic is one static Go binary. No client-server pair, no daemon, no database to manage.

```
restic -r sftp:backup@host:/repo backup ~
restic -r sftp:backup@host:/repo restore latest --target ~
```

### Verified restores

Snapshots are verified by default. A backup you cannot restore is not a backup, and restic treats restoring as a first-class command.
