# Gallery folder

Your 7 photos and 7 clips are already in here, web-compressed. The site finds them
automatically and shows them as scrolling rows — no code changes needed.

To add more, keep the numbering going with no gaps:

- Photos: `8.jpg`, `9.jpg`, … (`.png` also works)
- Clips:  `8.mp4`, `9.mp4`, …

Two rules for clips:
1. They must be **H.264** mp4s. iPhones record HEVC by default, which browsers can't
   play — convert first (e.g. with HandBrake, preset "Web > Vimeo YouTube 720p"), or
   set iPhone camera to "Most Compatible" format.
2. Keep them small — under ~5 MB loads fast; GitHub refuses files over 100 MB.

The site stops looking at the first missing number, so don't skip any.
