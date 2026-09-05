# Super Mario Bros. Movie – Dutch Dub

This repository contains a GitHub Actions workflow to automatically download the 1080p Blu-ray of *The Super Mario Bros. Movie* (2023), replace the audio with the Dutch dub, and produce a playable file.

## Why not full original quality on Catbox?

- **Catbox.moe** permanent uploads are limited to **200 MB**.
- The original 1080p HEVC + Dutch audio is ~2.3 GB.
- Therefore the workflow produces a high-quality re-encoded 1080p version that stays under practical limits (or a 720p version for permanent Catbox).

## How to use

1. Put `Dutch.mp3` in the root of this repository (or change the path in the workflow).
2. Go to the **Actions** tab → select **Sync Dutch Dub** → **Run workflow**.
3. When finished, download the artifact.

You can also edit the workflow to upload the result to Litterbox (temporary, up to 1 GB) if you prefer a direct link.

## Notes

- The original video source is the Pahe.in 1080p UHD BluRay release.
- Audio is the provided Dutch dub (stereo).
- The workflow frees disk space first so the large download fits on the runner.
