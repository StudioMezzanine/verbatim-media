# verbatim-media

Public files for Verbatim's social posts. Metricool fetches each post's videos and images from here when it publishes, so everything in this repo is already meant for the public.

Verbatim teaches vocabulary from classic books, each word shown in the line it was written in. [Verbatim on the App Store](https://apps.apple.com/app/id6769495422).

## Layout

```
posts/
  YYYY-MM-DD-<word>/
    slide1.mp4 … slide3.mp4   3-slide carousel, 1080 × 1920, 10 s seamless loops with sound (Instagram)
    slide1.png … slide3.png   the same slides as stills (Pinterest carousel)
    slide1.jpg … slide3.jpg   the stills as JPEG (TikTok photo carousel)
    reel.mp4                  18 s swipe through all three slides with sound (YouTube Shorts, morning Instagram Reel)
    captions.json             post ID, scheduled time, the caption, title and tags for each network, plus the quote and its source
```

Each post is made for one platform, so a folder holds only the files that platform needs:

| Platform | Files |
|---|---|
| Instagram + Threads | slide1–3.mp4 (moving carousel), slide1–3.png; the morning Instagram post (ID ending -02) also has reel.mp4 and goes out as a Reel |
| TikTok | slide1–3.jpg (photo carousel) |
| YouTube Shorts | reel.mp4, slide1.png |
| Pinterest | slide1–3.png (carousel pin) |

Metricool fetches each post's files straight from its folder on this branch.

## Rules every post follows

- The quote matches the public-domain text word for word; `captions.json` records where it was checked.
- Example sentences are written fresh and labelled as examples, never presented as from the book.
- Sound is generated for each scene (no music, no stock): about -22 LUFS outdoors, -25 LUFS indoors, true peak below -3 dBTP, and every loop joins cleanly.
- UK English, no em dashes.

Files are added by Studio Mezzanine's posting pipeline. Please don't edit posts that are already scheduled.
