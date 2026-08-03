## ly

A display manager with a console UI.

ly draws a text login screen on the TTY and starts the session you choose, including Wayland compositors.

### Lightweight, TUI

ly is a single C binary with a console interface.

No compositing, no desktop-environment dependencies, no daemon farm.

### Session list

Pick a session from the list, type your password, and go.

It reads the same session files that other display managers read.

### A minimal greeter

ly is the middle ground between emptty and the heavyweight greeters.

It stays on the TTY, keeps the code small, and does the one job of logging you in.
