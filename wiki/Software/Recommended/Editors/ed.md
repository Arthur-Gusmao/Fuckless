## ed

The original Unix text editor.

ed is the editor that shaped Unix.

Small, scriptable, and line-oriented, it established many of the ideas that would later influence ex, vi, sed, and countless other text-processing tools.

### Line-oriented by design

ed does not show a screen full of text. It operates on lines, one at a time.

The current line is always known, and addresses refer to lines relative to it. This model feels foreign today, but it is honest: a line is the unit the Unix tools were built around.

### Composable and scriptable

ed is not just interactive. It reads commands from its input, which means the same language you type by hand can be written to a file and executed.

Whole editing sessions become scripts, and ed can be dropped into pipelines with other tools.

### Standard, tiny, and everywhere

ed is one of the few text editors specified by POSIX.

Its implementation is measured in hundreds of lines, and it runs almost anywhere a C compiler does. When nothing else is available, ed is still there.

### The root of everything

ex, vi, sed, and grep all trace their lineage back to ed's ideas.

Learning ed is not about using an obsolete tool. It is about understanding the foundation that modern text processing stands on.