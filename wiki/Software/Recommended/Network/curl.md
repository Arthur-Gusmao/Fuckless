## curl

The command-line tool for transferring data with URLs.

curl speaks every protocol most people will ever need: HTTP, HTTPS, FTP, IMAP, SMTP, and more, from one interface.

### The universal pipe in and out

curl writes the body to stdout unless told otherwise, so it composes with everything:

```
curl https://example.com/feed.xml | sfeed
curl -o backup.tar.gz https://server/backup.tar.gz
```

It is the network analog of cat: a small program that moves bytes between a URL and your terminal.

### One tool, many protocols

A single binary with no daemon and no GUI. The feature surface is wide, but each flag does one thing and is documented.

For a wiki that values one tool doing one job well, curl is the transfer tool.

### Minimal to run

curl is a static binary with no runtime dependencies and no background service.

It is the thing sfeed and scripts use to fetch, which keeps the whole stack composable.

### Battle-tested

curl is everywhere, audited for decades, and portable to every Unix.

The more boring and reliable a tool is, the better it fits here.
