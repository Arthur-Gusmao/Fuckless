## hst

A terminal emulator built on neuwld.

hst is a pre-patched, freeway-compatible version of st-wl, with better font rendering thanks to neuwld.

### st-wl, improved

The base is st-wl, the Wayland port of st.

The neuwld drawing library fixes what the original wld did badly, starting with fonts that no longer hurt the eyes.

### A neulibs terminal

hst renders through neuwld, the same drawing library that the neuswc compositors use.

The whole stack shares one small foundation.

### Part of a coherent desktop

hst is the terminal of the neulibs ecosystem.

It pairs with the neuswc compositors and the other neuwld programs in this section.
