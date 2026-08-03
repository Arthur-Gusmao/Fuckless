## Kakoune

A modal code editor built around selections instead of cursors.

Kakoune rethinks modal editing from first principles.

Instead of extending Vim's model, it inverts it: selections come first, commands come second.

The result is an editor that is both simpler and more expressive.

Kakoune demonstrates that modal editing can evolve without accumulating decades of historical baggage.

Its design is consistent, composable, and centered around manipulating selections rather than moving cursors.

### Selection-first editing

In Vim, the typical workflow is:

> move → select → operate

In Kakoune, it becomes:

> select → operate

This makes editing feel more natural, especially when working with multiple selections.

### Multiple selections

Multiple cursors are a core feature, not an extension.

Editing dozens of locations simultaneously requires no plugins or complex configuration.
