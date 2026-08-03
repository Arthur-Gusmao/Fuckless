## river

A non-monolithic Wayland compositor.

river does not combine the compositor and the window manager into one program.

Instead, the compositor renders, and a separate window manager decides the policy. Any window manager implementing the `river-window-management-v1` protocol can be used.

### Compositor and window manager separated

river defers all window management policy to a separate process: window position and size, pointer and keyboard bindings, focus management, decorations, and desktop shell graphics.

The compositor itself focuses on frame-perfect rendering, protocol support, and Xwayland. This separation keeps the compositor small and the policy user-owned.

### An external window manager

The user chooses a window manager that speaks the river protocol.

This lowers the barrier to writing a window manager, allows implementations in high-level languages, and lets users hot-swap designs without restarting the desktop.

### Recommended window managers

The community maintains many river-compatible window managers. The following are small, keyboard-driven, and in the spirit of this wiki — no bars, no panels, no Python:

- [anvl](Window-Managers/anvl.md) — minimal dwm-style tiling, in C
- [crofflewm](Window-Managers/crofflewm.md) — static tiling, in Go
- [orilla](Window-Managers/orilla.md) — XMonad-inspired dynamic tiling, in Rust
- [rijan](Window-Managers/rijan.md) — dynamic tiling in 600 lines of Janet, by the river author
- [rill](Window-Managers/rill.md) — minimalist scrolling layout, in Zig
- [ropotamo](Window-Managers/ropotamo.md) — StumpWM-like window management, in Janet
- [tinyrwm](Window-Managers/tinyrwm.md) — the official examples, a starting point for your own window manager
- [zrwm](Window-Managers/zrwm.md) — dynamic tiling configured from the command line, in C

### Written in Zig

river is written in Zig, a small systems language that keeps the codebase readable and free of the baggage of older languages.

It runs on both Linux and BSD, staying portable rather than Linux-bound.

### river-classic

The original version of river, now maintained separately as river-classic, was the old dynamic tiling design.

It is the one that used `riverctl` for configuration and `rivertile` as its layout generator, arranging windows in a tiled layout in the tradition of dwm, xmonad, and bspwm.

When river was redesigned as a non-monolithic compositor, river-classic was kept and packaged separately for users who prefer the older design.
