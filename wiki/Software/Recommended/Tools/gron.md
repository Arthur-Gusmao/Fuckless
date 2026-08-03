## gron

Make JSON greppable.

gron transforms JSON into discrete path assignments, one per line, so you can search it with `grep` instead of a query language.

### JSON as text

Each value becomes a line showing its path:

```
json[0].commit.author.name = "Tom Hudson";
```

Then the tools you already know apply: `grep`, `sed`, `cut`.

### Round-trip

Filtered output can be converted back to JSON with `--ungron`, so gron is also a way to build JSON from the shell.

### A single binary

Written in Go, no runtime dependencies.

It does not replace jq; it replaces the need to learn a query language to answer one question.
