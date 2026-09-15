# AnyDownload

Paste any video link. Download it straight to your phone.

AnyDownload is a lean, local video downloader for Android. It embeds the
[yt-dlp](https://github.com/yt-dlp/yt-dlp) extraction engine plus ffmpeg and
aria2c, so **everything runs on your device** — no cloud, no servers, no
account, no ads, no tracking.

- **1,000+ sites** supported by yt-dlp: YouTube, TikTok, Instagram, X/Twitter,
  Reddit, Facebook, Vimeo, Twitch, SoundCloud, Bilibili and many more
- **Any quality** — up to 4K/8K where the source provides it
- **Any type** — video, audio (mp3/m4a), thumbnails, playlists
- Paste a link *or* share a link into the app from any other app
- Downloads land in `Download/AnyDownload/`
- 100% on-device: your links never leave your phone

Based on [YTDLnis](https://github.com/deniscerri/ytdlnis) (GPL-3.0).

## Install

1. Download the APK for your phone from the
   [latest release](https://github.com/m55681518-byte/AnyDownload/releases/latest):
   - **arm64-v8a** — all modern phones (Samsung, Pixel, Xiaomi, OnePlus, ...)
   - **universal** — anything else / old devices
2. Open the APK file. Android asks once to allow *install from unknown sources* — tap **Allow**.
3. Open AnyDownload, paste a link, hit the download button.

> AnyDownload is not on Google Play. Play Store policy bans video-downloading
> apps, so this is distributed as a sideload APK from GitHub releases, like
> Seal and other apps in this category.

## Usage

- **Paste a URL** on the home screen and press search — the app analyzes the
  link, shows quality options, and downloads.
- **Share to AnyDownload** — from YouTube, TikTok, Instagram or any app, tap
  *Share* → *AnyDownload*, and the link opens ready to download.
- **Playlists / channels** — paste a playlist link to batch download.

## Updating

When platforms update their anti-downloader measures, download engines need
refreshing. Check the
[releases page](https://github.com/m55681518-byte/AnyDownload/releases) for
the newest build and install the new APK over the old one (your downloads are
kept).

### Auto updates (optional)

Use [Obtainium](https://obtainium.imranr.dev) and add this repo:
`https://github.com/m55681518-byte/AnyDownload` — it will track releases and
offer in-app updates.

## Troubleshooting

- **Site stopped working** → a newer engine may be needed; update the app.
- **Permission denied** → android 10+ uses MediaStore; grant storage access
  when prompted. Older Android versions require Storage permission.
- Anything else → open an issue with the app log (More → Logs).

## Build from source

```bash
git clone https://github.com/m55681518-byte/AnyDownload.git
cd AnyDownload
# requires JDK 17 and the Android SDK
./gradlew assembleGithubRelease
```

APKs land in `app/build/outputs/apk/github/release/`.

## License

GPL-3.0. Third-party components: yt-dlp (Unlicense), ffmpeg (GPL), aria2c
(GPL), and the libraries listed in the original project.