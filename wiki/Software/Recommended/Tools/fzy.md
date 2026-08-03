## fzy

A fast, simple fuzzy text selector for the terminal.

fzy reads a newline-separated list from stdin and lets you pick one with a smart scoring algorithm.

### A better match

Most fuzzy matchers sort by match length.

fzy scores matches on consecutive letters and word starts, so `amp` finds `app/models/posts.rb` rather than a random string. It finds what you intended.

### stdin in, answer out

A drop-in for selecta, fzy composes with anything that prints lines:

```
find . -type f | fzy
```

### Small C

One small C program, no dependencies, fast on large lists.
