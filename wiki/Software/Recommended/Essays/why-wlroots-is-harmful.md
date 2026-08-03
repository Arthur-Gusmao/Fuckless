## Why wlroots is harmful

wlroots is the most popular way to build a Wayland compositor.

Popularity is not the same as quality.

This wiki is opinionated, and our position is that wlroots works against everything the software listed here stands for. Here is why.

### It is huge

wlroots is often described as "60,000 lines of code you were going to write anyway."

In reality it is closer to 80,000 lines.

The promise behind that slogan is false. A compositor library does not need to be that big. swc, the library behind the neulibs compositors in this wiki, shows that a working, hackable foundation can be written in a fraction of the code.

Every line of a library is a line you do not control. Every line is a design decision someone else made for you.

### It drags in protocol bloat

wlroots does not just provide compositing.

It pulls in a large set of protocol extensions, some of which are large and badly designed. The user pays for all of them whether they use them or not, in code size, compile time, and complexity.

### It is Linux-centric

wlroots is deeply tied to Linux: udev for device handling, and a particular model of seat management.

On BSD it does not work natively. It needs compatibility shims, which is a polite word for hacks.

A foundation that cannot run on more than one Unix-like system is not portable. Portability is one of the requirements of this wiki.

### It moves too fast

wlroots changes frequently and breaks compatibility without ceremony.

Small projects built on it are abandoned not because their ideas failed, but because their developers could not keep up with the churn. The wayland.fyi page on wlroots lists abandoned hobby compositors as direct casualties of this pace.

A fast-moving dependency is a treadmill. You spend your time tracking its changes instead of doing your own work.

### It is low-level, and still hard

For all its size, wlroots remains low level.

Writing a compositor with wlroots is still a lot of work, which is why so few people attempt it. A library that is simultaneously huge and low level has the worst of both worlds: too much to understand, and not enough help.

### The cost of a single big dependency

When your entire desktop rests on one large library, you are locked in.

Its design decisions become yours. Its bugs become yours. Its direction becomes yours. You can no longer read, understand, or meaningfully modify the foundation of your system.

That is the opposite of user control.

### There is a better way

The compositors in the neulibs section of this wiki prove that a small, portable, readable compositor library is possible.

swc and its fork neuswc keep the whole stack small enough to audit, work natively on BSD, and do not churn underneath you.

Software that needs a massive foundation to justify its existence does not belong in a wiki about minimal software. wlroots is the clearest example of that.

### A pragmatic note

This wiki is not dogmatic. We still recommend a few wlroots-based compositors, such as dwl, river, and cage.

The neulibs ecosystem is still experimental. swc and neuswc are smaller and more auditable, but they do not yet cover the practical ground of a daily desktop. Screensharing is missing or incomplete, and the rendering stack has not caught up with what games and other demanding applications expect.

Until the neulibs compositors are ready for those workloads, a few wlroots compositors remain the pragmatic recommendation for users who need a working desktop today.
