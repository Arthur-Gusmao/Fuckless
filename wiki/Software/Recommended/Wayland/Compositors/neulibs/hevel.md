## hevel

A floating, scrollable compositor inspired by Plan 9 user experience, built on neuswc.

hevel takes its cues from Plan 9.

Windows float instead of being forced into tiles, and the workspace scrolls rather than stacking pages of windows. It is the Plan 9 model of the desktop, brought to Wayland.

### Plan 9 influence

In Plan 9, the window system does not pretend to be a desktop environment.

Windows are simply there, positioned by the user. hevel keeps that spirit: few decorations, few rules, and no interference in how windows relate to each other.

### Scrollable workspace

Instead of virtual desktops, hevel gives you one continuous workspace that scrolls.

Rather than managing dozens of desktop pages and their rules, you move through a single space. Less machinery, fewer concepts.

### Built on neuswc

hevel is built on neuswc, the feature-correct fork of swc.

That means a compositor library small enough to understand, with none of the weight of mainstream alternatives.
