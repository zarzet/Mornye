<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/readme/banner-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/readme/banner-light.svg">
  <img alt="Mornye. Your music. Every detail." src="assets/readme/banner-light.svg" width="760">
</picture>

<p>
  <a href="CHANGELOG.md"><img alt="0.1" src="https://img.shields.io/badge/version-0.1-596554?style=for-the-badge"></a>
  <a href="#availability"><img alt="Native for Mac and iPhone" src="https://img.shields.io/badge/Mac_%26_iPhone-Native-363833?style=for-the-badge&amp;logo=apple&amp;logoColor=white"></a>
</p>

<p><strong>Your local music, with lossless playback, synced lyrics, and daily mixes. Built for Mac and iPhone.</strong></p>

<p><a href="https://mornye.com">Website</a> · <a href="CHANGELOG.md">Changelog</a> · <a href="SUPPORT.md">Support</a> · <a href="https://mornye.com/privacy.html">Privacy</a></p>

</div>

Mornye gives your local music a home on Mac and iPhone. Import your files, explore albums and artists, follow the lyrics, and find something to play through Daily Sessions shaped by your library and listening habits.

Local playback works offline, without an account. Your music and listening profile stay on your device.

> [!NOTE]
> **0.1 is being prepared.** Public downloads are not available yet. The interface and features are still being polished. Official download or TestFlight links will appear on [mornye.com](https://mornye.com/#download) when available.

## Screenshots

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/readme/mac-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="assets/readme/mac-light.svg">
    <img src="assets/readme/mac-light.svg" alt="Mornye Home on Mac, with Top Picks, Daily Sessions and the player bar" width="760">
  </picture>
</p>

<p align="center">
  <img src="assets/readme/iphone-dark.svg" alt="Mornye Home on iPhone in dark mode" width="230">
  <img src="assets/readme/iphone-light.svg" alt="Mornye Home on iPhone in light mode" width="230">
</p>

<p align="center"><sub>Mac and iPhone previews. Music and artwork shown are examples from a personal library; no music is bundled with Mornye.</sub></p>

## Availability

| Platform | Minimum system | Status |
| --- | --- | --- |
| Mac | macOS 26 or later | 0.1 in preparation |
| iPhone | iOS 26 or later | 0.1 in preparation |
| Windows | To be announced | Support will follow |
| Android | To be announced | Support will follow |

Windows and Android do not have a release date or downloadable build yet. Download availability will be announced through the official website and this repository.

## Features

### Your library, organized

- Import music from Files or Finder; drag files into the Mac app or open them with Mornye.
- Choose a music folder and scan its subfolders. Scan again to add new or changed files while skipping unchanged duplicates.
- Change or disconnect the source folder without removing music already imported.
- Refresh song metadata, remove individual songs, or clear the library with confirmation. Original source files stay untouched.
- Browse albums, artists, recently added music, favorites, genres, years, composers, labels and formats.
- Create playlists with custom covers and descriptions. Manage the play queue with Play Next, Play Last, reordering and removal.
- Pick up where you left off: your queue, current song, playback position, shuffle and repeat settings are saved across app restarts. Playback stays paused until you resume.

### Something for today

**Daily Sessions** build selections from the music you already own. Sessions reflect the tags and variety in your library, with on-device learning from the music you choose, replay and skip.

Selections stay stable during the day and refresh on a new day. A smaller collection can produce fewer sessions. Local AutoPlay can suggest what to hear next, and listening-based learning can be disabled or reset in Settings.

### Lyrics that follow along

Read embedded lyrics or add your own. Mornye supports plain lyrics, synchronized LRC, word-timed LRC, and supported TTML timing.

Place a `.lrc` or `.ttml` file beside the song with the same filename before importing, or attach lyrics later through **Edit Lyrics → Import Lyrics**. Select a timed line to seek to that point in the song.

Lyrics come from your files. Mornye does not include an online lyrics catalog.

### Sound with clear information

- Lossless and high-resolution source playback, with source format and device output shown separately in **Now Playing → Audio Quality**.
- ReplayGain **Track** and **Album** modes, with preamp and clipping protection for appropriately tagged files.
- Opus and Vorbis decoding built in; no external conversion app is required.
- Native media controls, background local playback on iPhone, and a separate MiniPlayer window on Mac.
- AirPlay through the system output controls and experimental Google Cast support for local files.

### A native place to listen

Light, dark and system appearances; artwork-led browsing; horizontally scrolling shelves; and a compact player that keeps the music close. iPhone navigation adapts as you scroll, while Mac provides a sidebar, keyboard controls and a Dock menu.

## Supported audio

| Format / container | Audio supported |
| --- | --- |
| `.opus` | Ogg Opus |
| `.ogg`, `.oga` | Ogg Vorbis; Ogg Opus is detected from its contents |
| `.m4a`, `.m4b`, `.mp4` | AAC or Apple Lossless (ALAC) in supported audio containers |
| `.flac` | FLAC |
| `.wav`, `.wave` | Supported WAV audio, including PCM |
| `.aif`, `.aiff`, `.aifc` | Supported AIFF audio |
| `.mp3` | MP3 |
| `.aac`, `.adts` | AAC |
| `.caf` | Supported Core Audio Format audio, including PCM |

**M4A is a container, not a quality level.** An AAC file is lossy; an ALAC file is lossless. Mornye identifies the actual codec rather than guessing quality from the extension. The Hi-Res Lossless label appears only for qualifying lossless source files.

Opus and Vorbis are prepared as separate PCM playback copies during import. This uses additional storage while preserving the original file. Their quality labels remain **Opus** or **Vorbis**; decoding does not make lossy audio lossless.

M4B files are imported as audio tracks; audiobook chapter navigation is not available. Supported codecs vary by container.

## Getting started

Once an official build is available:

1. Install it from the link on [mornye.com](https://mornye.com/#download).
2. Open Mornye and choose **Import Music**.
3. Select audio files available on your device. Mornye copies them into its library.
4. Browse your albums or play a song. Daily Sessions appear once enough music has been added.
5. Open **Settings → Library Settings** to choose a source folder, scan it again, refresh metadata or remove imported songs.

**Scanning and refreshing do different jobs.** Scan Music Folder checks the selected source folder for new or changed files. Refresh Songs rereads metadata from Mornye’s existing imported copies.

Removing music from Mornye removes its local copies and playlist references. It does not delete the source files. Scanning the same source folder later can add those songs back.

## Privacy

Mornye has no account requirement, advertising or analytics SDK. Library metadata, playlists, preferences and listening-based personalization are stored locally. The publisher does not receive your library or listening history automatically.

When you choose a Cast receiver, Mornye sends the selected audio and its metadata to that receiver over your local network. AirPlay is handled by the operating system. Support links open your browser or email app; you choose what information to share.

Read the [privacy policy](https://mornye.com/privacy.html) for details on local data, backups, deletion and optional network use.

## Release notes

The first version is a starting point, and polish is ongoing. Current limits include:

- Output quality depends on the operating system, connection and audio device. Exclusive bit-perfect hardware output and guaranteed gapless playback are not claimed.
- AirPlay and Google Cast still need broader physical-device testing. Keep Mornye open when casting local files; background Cast hosting is not guaranteed.
- No published Windows or Android build yet.

Bugs, rough edges and behavior changes are possible in this early version. See [CHANGELOG.md](CHANGELOG.md) for the current development notes.

## FAQ

<details>
<summary><b>Does it work offline?</b></summary>

Yes. Imported music, lyrics and on-device recommendations work offline. Wireless receivers and external links need their respective connections.

</details>

<details>
<summary><b>Why is my library empty on first launch?</b></summary>

Mornye does not bundle songs. Choose Import Music to add your own files. The screenshot library is not included with the app.

</details>

<details>
<summary><b>Do Daily Sessions change every time I open Home?</b></summary>

No. Your daily selection is saved for the day. Sessions can change on a new day as your collection and listening habits develop. Removing unavailable songs can also change what remains playable.

</details>

<details>
<summary><b>Why does a high-resolution file play at a different output rate?</b></summary>

Source quality and device output are different. The system or connected device may resample audio, and Bluetooth may use lossy compression. Check Audio Quality in Now Playing. On Mac, configure a compatible DAC through Audio MIDI Setup.

</details>

## Feedback and contributions

[Report a bug](https://github.com/zarzet/Mornye/issues/new?template=bug_report.yml) · [Suggest a feature](https://github.com/zarzet/Mornye/issues/new?template=feature_request.yml)

Bug reports, feature suggestions and documentation corrections are welcome. Please read [SUPPORT.md](SUPPORT.md) before reporting a problem and [CONTRIBUTING.md](CONTRIBUTING.md) before sending documentation changes.

Include the app version, device, operating system and steps to reproduce. Remove personal details from screenshots and logs. Do not attach private audio files or your entire library.

For private support, contact **[zarzet@mornye.com](mailto:zarzet@mornye.com)**. Potential security issues should be reported privately using [SECURITY.md](SECURITY.md).

## About Mornye

Mornye is developed by **Zarz Eleutherius**. Follow this repository for release notes, share feedback, and help shape future updates.

If you would like to support development:

[![Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/zarzet)

Use **Watch → Custom → Releases** on GitHub to receive release announcements once releases are published.
