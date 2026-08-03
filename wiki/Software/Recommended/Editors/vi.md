## vi

The standard Unix visual editor.

vi introduced visual screen editing to Unix while preserving the simplicity and composability of its predecessor, ex.

More than forty years later, its editing model continues to influence countless editors.

### A tiny core

vi began as a small program on top of ex.

Its whole design fits in a modest amount of code, yet it provides editing that professionals have relied on for half a century. There is no plugin system, no scripting language, and no configuration directory. There does not need to be.

### The modal model

vi made a simple but powerful choice: separate editing from inserting text.

Normal mode interprets every key as a command, insert mode types. Because commands are single keystrokes, editing becomes a vocabulary of verbs and motions that compose without extra ceremony.

### Composable commands

Everything in vi composes.

A movement, a count, and an action combine into a single instruction: `d2w` deletes two words. This small grammar is what makes the editor so expressive, and why the model has survived every trend since.

### It is everywhere

vi is standardized and available on virtually every Unix-like system.

When a remote system has nothing else, it still has vi. Knowing vi means never being without an editor.
