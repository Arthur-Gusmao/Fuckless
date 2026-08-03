## toybox

All-in-one minimal command line utilities.

toybox implements the standard Unix tools in a single small binary.

### One binary, many tools

`toybox` contains cat, ls, cp, sed, find, grep, and hundreds more, selected by the first argument:

```
toybox ls
toybox cp a b
```

### Built for small systems

toybox is designed for embedded systems where GNU coreutils cannot fit.

That constraint keeps the code honest: each tool is the minimum that does the job.

### Readable source

Every utility is a separate file that can be read on its own.

It is a practical, maintained alternative to the sbase ideal.
