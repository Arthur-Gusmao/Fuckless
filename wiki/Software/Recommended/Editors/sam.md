## Sam

A structural text editor created by Rob Pike for Plan 9.

Sam is one of the most influential text editors ever written.

Rather than relying on modes, plugins, or complex configuration, Sam focuses on one idea: editing text should be precise, composable, and programmable.

Sam demonstrates that an editor can remain small while providing editing capabilities that many modern editors still struggle to match.

Its command language treats text as a structured object rather than a sequence of keystrokes.

### Structural editing

Sam operates on text through addresses and commands.

Instead of repeatedly moving the cursor and executing commands, users describe what they want to edit.

Editing becomes declarative rather than procedural.

### A real command language

Sam's editing language is consistent and expressive.

Complex transformations that require plugins, macros, or scripting in other editors are often simple one-line commands.
