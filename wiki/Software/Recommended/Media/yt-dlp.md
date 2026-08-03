## yt-dlp

A command-line program to download videos and audio.

yt-dlp fetches media from hundreds of sites, extracts the streams, and saves them. It is the fork of youtube-dl that is still maintained.

### The extraction tool

yt-dlp reads a URL, finds the media, and writes the file:

```
yt-dlp URL
yt-dlp -x --audio-format mp3 URL
yt-dlp -f bestvideo+bestaudio URL
```

The output format is chosen per-command; nothing plays in a GUI and nothing runs in the background.

### Text in, files out

It is a pipeline tool: input is a URL, output is a file on your disk.

That makes it composable with scripts, cron, and a music manager like cmus.

### One binary

yt-dlp is a single Python package that runs everywhere Python does.

No account, no app store, no tracking. You decide which videos you keep, in what quality.

### The maintained fork

The original youtube-dl stopped keeping up with the sites; yt-dlp continues that work.

It is the version that still does the one thing: download the media you point it at.
