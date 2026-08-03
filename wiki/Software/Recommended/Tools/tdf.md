## tdf

A PDF viewer for the terminal.

tdf renders PDFs directly inside a terminal emulator, with asynchronous rendering, search, and responsive layout.

### No window needed

tdf draws pages into the terminal, so there is no separate window to manage.

Reading a PDF becomes a terminal task, the same as editing a file or running a shell command.

### Fast on large documents

Rendering is asynchronous, so scrolling and searching stay responsive even on big PDFs.

Progress of rendering and search is shown while the document loads.

### Search built in

Full text search is part of the viewer, with highlighting and jump-to-result.

A PDF is a document to be read, not just a paper to look at.

### Written in Rust

Built on ratatui and poppler, this is an original project rather than a rewrite of an existing tool.

Small enough to fit the terminal workflow of this wiki.
