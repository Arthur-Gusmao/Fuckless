## ffmpeg

The command-line tool for converting audio and video.

ffmpeg reads media from files or stdin and writes it anywhere, doing the demuxing, decoding, and encoding itself with no GUI and no daemon.

### One command, every format

```
ffmpeg -i in.mkv out.mp4
ffmpeg -i in.mkv -vn out.mp3
ffmpeg -f x11grab -i :0 out.mkv
```

The same binary handles capture, conversion, and streaming.

### Text in, text out

ffmpeg is a pipeline tool in the Unix tradition: it reads and writes streams, takes options, and prints diagnostics to stderr.

It composes with everything, which is why scripts drive it.

### A library with a CLI

At its core is libavcodec and the av framework, a set of C libraries.

The `ffmpeg` binary is the small interface over them, and the libraries are what other minimal tools link against.

### No bloat in the running program

No installer, no GUI, no background service.

One static-ish binary that does the job and exits, leaving the machine the way it found it.
