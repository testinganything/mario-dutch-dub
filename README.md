# Super Mario Bros. Movie – Dutch Dub (Original Quality)

This repository automatically creates a **true original-quality** version of *The Super Mario Bros. Movie* (2023) with the Dutch audio track properly synced.

## What it does

- Downloads the original 1080p UHD BluRay (HEVC)
- Downloads the Dutch dub audio
- Muxes them with `-c:v copy` (no quality loss on the video)
- Forces both streams to start at the same timestamp → fixes the desync you saw in VLC
- Uploads the finished ~2.3 GB file to **Gofile.io**
- Also keeps it as a GitHub Actions artifact (3-day backup)

## How to use

1. Go to the **Actions** tab
2. Select **Sync Dutch Dub**
3. Click **Run workflow**
4. Wait for it to finish (can take 40–90 minutes)
5. In the job logs look for the green success message with the Gofile link (`https://gofile.io/d/xxxxxxxx`)

You no longer need to upload `Dutch.mp3` yourself — the workflow downloads it automatically.

## Notes

- Original video: Pahe.in 1080p UHD BluRay release
- Audio source: the catbox link you provided
- Output: MP4 (HEVC video + AAC audio) for best compatibility
- Free Gofile links can expire if the file is not downloaded for a long time — save a copy soon after the run finishes.
