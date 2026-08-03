## jq

A command-line JSON processor.

jq reads JSON, filters it, and rewrites it, from the shell.

### The sed for JSON

jq uses a small query language to select, transform, and reshape documents:

```
curl api | jq '.items[] | {name, price}'
echo '{"a":1}' | jq '.a'
```

It is the missing filter between raw data and the tools you already use.

### Streams in, streams out

jq reads from stdin and writes to stdout.

That makes it composable in pipelines, and its output is valid JSON you can feed to the next tool.

### A library for C

The `libjq` is a C library, and jq itself is a thin command-line program over it.

It is hackable and embeddable, the way this wiki likes its tools.

### Complements gron

Where gron flattens JSON into lines for grep, jq handles structured queries.

For scripts that need real JSON manipulation, jq is the tool.
