## mdp

A command-line presentation tool that renders Markdown slides in the terminal.

mdp reads a Markdown file, splits it into slides, and shows them full-screen with keyboard navigation. No browser, no export, no deck tool.

### Slides are plain text

The source is a Markdown file: headings, lists, code blocks, and quotes.

A horizontal rule separates slides. Your talk is a text file you already know how to write, version, and diff.

### Presentation in a terminal

mdp renders with ncurses and runs in any terminal.

The audience watches the same screen the presenter uses, which is enough for a talk without a projector.

### Keyboard navigation

Next, previous, first, last, and reload are keypresses.

There is nothing else to learn, because there is nothing else it does.

### Written in C

mdp is a small C program using ncurses.

It is the suave answer to "slides but without a GUI", and it fits a wiki that keeps its tools small.
