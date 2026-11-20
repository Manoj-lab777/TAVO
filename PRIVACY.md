# Tavo — Privacy

**Short version:** Tavo has no account, no ads, no analytics and no tracking.
Everything it remembers stays on your computer.

## What Tavo stores (only on your PC)
All in `%APPDATA%\Tavo`:
- `tavo.json` — your settings, library folders, where you stopped each video, sound sync per video.
- `thumbs\` — thumbnails Tavo made of your videos.
- `backgrounds\` — wallpaper pictures you chose.
- `tv\` — the downloaded channel lists and which channels answered.
- `extras.json` — your Live TV choices, your playlist link and recent stream links.
- `.vault` — your private channels, encrypted with your PIN.
- `tavo.log` — error messages (file names, never full web links with their access tokens), to help fix problems. Kept under 512 KB.
- `tools\` — yt-dlp and Deno, only if you set up web videos.

Uninstalling Tavo leaves this folder so you don't lose your settings; delete it to remove everything.

## When Tavo goes online
Only for features you use:
| What you do | Who Tavo talks to |
|---|---|
| Open Live TV | iptv-org (github.io) for channel lists, then each channel's own server to check it's on air and to play it |
| Open Radio | radio-browser.info, then the station's server |
| Play a stream or web link | that site's servers (and yt-dlp asks the site for the video) |
| Set up web videos / Update | github.com (yt-dlp and Deno releases) |
| Random wallpaper / picture link | picsum.photos or the link you gave |

Those servers see your IP address, like any website you visit. Tavo sends no
personal information, and nothing about what you watch, to the author.
