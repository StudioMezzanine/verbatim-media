# verbatim-media

Public files for Verbatim's social posts. Metricool fetches each post's videos and images from here when it publishes, so everything in this repo is already meant for the public.

Verbatim teaches vocabulary from classic books, each word shown in the line it was written in. [Verbatim on the App Store](https://apps.apple.com/app/id6769495422).

## Layout

```
posts/
  YYYY-MM-DD-<word>/
    slide1.mp4 … slide3.mp4   3-slide carousel, 1080 × 1920, 10 s seamless loops with sound (Instagram)
    slide1.png … slide3.png   the same slides as stills (Pinterest, Threads, TikTok photo mode)
    reel.mp4                  18 s swipe through all three slides with sound (TikTok, YouTube Shorts, Reels)
    cover.jpg                 cover frame for video posts
    captions.json             the caption, title and hashtags for each platform, plus the verified quote and its source
```

## Rules every post follows

- The quote matches the public-domain text word for word; `captions.json` records where it was checked.
- Example sentences are written fresh and labelled as examples, never presented as from the book.
- Sound is generated for each scene (no music, no stock): about -22 LUFS outdoors, -25 LUFS indoors, true peak below -3 dBTP, and every loop joins cleanly.
- UK English, no em dashes.

Files are added by Studio Mezzanine's posting pipeline. Please don't edit posts that are already scheduled.
