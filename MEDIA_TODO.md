# Media TODO

Two media slots are already in `index.html` but hidden, so the live site looks
normal until the files exist. Drop a file in, delete one class, done.

## Files to add

Put both in `assets/robot/`:

| File | Where it shows | Notes |
| --- | --- | --- |
| `yam_policy.mp4` | RESEARCH.LOG, the PAIR Lab entry | Autoplays muted on loop |
| `yam_policy_poster.jpg` | Poster frame for the video above | Shown before the video loads |
| `so101.jpg` | PROJECTS.DIR, the SO-101 Robot Learning card | Card is 16:9, cropped to fill |

## Format

**Video** — MP4, H.264 (AAC audio or none; it plays muted either way).
Keep it **under ~8 MB** and **15–30 seconds**. 1280x720 is plenty. The clip
loops, so pick a segment that reads fine when it jumps back to the start.

```bash
ffmpeg -i input.mov -t 25 -vf scale=1280:-2 -c:v libx264 -crf 28 -preset slow -an assets/robot/yam_policy.mp4
```

**Stills** — JPG, 1280x720 or larger, same 16:9 framing, quality ~80.

```bash
# poster frame grabbed from the video itself, at 2s
ffmpeg -i assets/robot/yam_policy.mp4 -ss 2 -frames:v 1 -q:v 3 assets/robot/yam_policy_poster.jpg
```

## Turning a slot on

Each slot has a `media-pending` class that hides it, and a `TODO` comment right
above it. Delete **only** the ` media-pending` from the class list.

Video, in the PAIR Lab research entry:

```html
<!-- TODO: add yam_policy.mp4 + yam_policy_poster.jpg, then remove media-pending -->
<div class="research-media media-pending">   <!-- becomes: class="research-media" -->
```

Image, in the SO-101 project card:

```html
<!-- TODO: add so101.jpg, then remove media-pending -->
<div class="project-image media-pending">    <!-- becomes: class="project-image" -->
```

Delete the `TODO` comment line at the same time. The SO-101 card's text is
visible already — only its image is waiting.

Check it locally before pushing, since a missing file shows a broken-media icon
once the class is gone:

```bash
python3 -m http.server 8000
```
