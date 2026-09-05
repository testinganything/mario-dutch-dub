# Super Mario Bros. Movie – Dutch Dub (Original Quality)

This repository contains a GitHub Actions workflow that creates a **true original-quality** version of *The Super Mario Bros. Movie* (2023) with the Dutch audio track perfectly synced.

## What it does

- Downloads the original 1080p UHD BluRay (HEVC)
- Replaces the audio with the Dutch dub (`Dutch.mp3`)
- Keeps the **exact original video stream** (`-c:v copy`) → no quality loss
- Uploads the finished ~2.3 GB file to **Gofile.io** and also keeps it as a GitHub artifact

The Dutch audio is fully synced because both the video and audio streams start at timestamp 0 and their durations match very closely.

## How to use

1. Add `Dutch.mp3` to the **root** of this repository (one-time step).
2. Go to the **Actions** tab → select **Sync Dutch Dub** → **Run workflow**.
3. Wait for it to finish (can take 30–90 minutes depending on download speed).
4. In the job logs, look for the green success message with the Gofile link (`https://gofile.io/d/xxxxxxxx`).
5. You can also download the file from the Artifacts section as a backup.

## Notes

- Original video source: Pahe.in 1080p UHD BluRay release.
- Audio: Dutch dub (stereo).
- Output container: MP4 (HEVC video + AAC audio) for maximum compatibility.
- Free Gofile links can expire if the file is not downloaded for a long time. Download it soon after the run finishes.
