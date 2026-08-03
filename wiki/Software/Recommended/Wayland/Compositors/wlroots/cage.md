## cage

A Wayland kiosk.

cage runs a single maximized application and nothing else.

It is a compositor whose entire scope is one window, fullscreen, with no window management to speak of.

### One application

Cage displays a single application at a time and prevents interaction with anything else.

There are no windows to tile, float, or decorate, which means there is no code for any of that. What is omitted cannot misbehave.

### Minimal footprint

The whole compositor fits in roughly a dozen C files.

That makes it trivial to audit and suitable for embedded systems, digital signage, and any appliance that should only ever show one thing.

### Built on wlroots

Cage inherits its protocol and input handling from wlroots.

Rather than reimplementing display plumbing, it adds only the small policy layer that a kiosk needs, keeping the whole program tiny.
