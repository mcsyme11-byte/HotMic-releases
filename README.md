# Hot Mic

**Free, private dictation for Windows.** Press **F9**, speak, and press **F9** again: clean, punctuated text appears at the cursor in any application, including Microsoft Word, web browsers, Discord and email.

Speech is processed entirely on the computer. Hot Mic needs no account and no subscription, and it contains no tracking.

**[Download Hot Mic for Windows](https://github.com/mcsyme11-byte/HotMic-releases/releases/latest/download/HotMic-Setup.exe)** · [Website](https://mcsyme11-byte.github.io/HotMic-releases/) · [All releases](https://github.com/mcsyme11-byte/HotMic-releases/releases)

> This repository hosts the official downloads, release notes and download website for Hot Mic. The source code is maintained privately.

---

## Features

- **Works in any application:** the text is typed at the cursor, wherever it is.
- **On-device AI:**
  - NVIDIA Parakeet speech recognition, with OpenAI Whisper as a second listener for muffled microphones such as Bluetooth headsets.
  - SpeakoFlow Mini, which removes filler words, repetitions and self-corrections.
  - All of them run locally.
- **Natural formatting:** spoken numbers, times, prices and years are written as digits ("at eight thirty" becomes "at 8:30"), and custom words are always spelled correctly.
- **Voice commands:** "new line", "new paragraph", "scratch that" and "press enter".
- **Designed for low vision:**
  - distinct sound cues for each step;
  - an optional large, high-contrast indicator;
  - read-back of the dictated text;
  - full keyboard and screen-reader support.
- **Light on system resources:** a Performance setting reduces Hot Mic's use of the graphics card and processor automatically while games or flight simulators are running.
- **Automatic updates** for installed copies, applied the next time Hot Mic starts.

## Downloads

| File | Description |
|---|---|
| **HotMic-Setup.exe** | The recommended installer. It installs Hot Mic for the current Windows user (no administrator rights required), adds Start menu and desktop shortcuts, and registers Hot Mic in Settings › Apps for uninstalling. Installed copies update automatically. |
| **HotMic.exe** | The complete application as a single file, for use without installation. This version does not update automatically. |
| `HotMicApp-*.nupkg`, `releases.win.json` | Update packages used by installed copies of Hot Mic. They do not need to be downloaded manually. |

## System requirements

- Windows 10 or Windows 11, 64-bit
- A microphone (headset, webcam or built-in laptop microphone)
- About 2 GB of free disk space for the AI models, which are downloaded once on first start
- Optional: a dedicated graphics card. It improves speed, and with 6 GB or more of graphics memory it enables Whisper for muffled microphones.

## Installation

1. Download **HotMic-Setup.exe** and open it.
2. If Windows displays **"Windows protected your PC"**, select **More info**, then **Run anyway**. The warning appears because Hot Mic is new and is not yet signed with a commercial code-signing certificate; it does not indicate a problem with the software.
3. Hot Mic starts automatically. In the Welcome window, select **Download** to fetch the free AI models (about 1.3 GB, once).
4. Place the cursor in any text field, press **F9** and speak.

**To uninstall:** Windows Settings › Apps › Installed apps › Hot Mic › Uninstall. Settings (`%APPDATA%\HotMic`) and the AI models (`%LOCALAPPDATA%\HotMic`) are kept, so that a reinstall does not download them again; these folders may be deleted manually.

## Privacy

Audio and dictated text never leave the computer. Hot Mic connects to the internet only:
- to download its AI models from Hugging Face, once;
- to check GitHub for updates, at most every 12 hours.

See the full [Privacy Policy](https://mcsyme11-byte.github.io/HotMic-releases/privacy.html).

## Terms and licences

Hot Mic is free to download and use, and is provided as is, without warranty. See the [Terms of Use](https://mcsyme11-byte.github.io/HotMic-releases/terms.html).

Hot Mic is built on open-source software and AI models, each under its own licence. See [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

## Support

Questions and problem reports may be sent to **Malcolm Syme** at [mcsyme11@gmail.com](mailto:mcsyme11@gmail.com).
- **When reporting a problem:** include the Hot Mic version (Settings › About) and, where possible, the log file. To open its folder: right-click the Hot Mic icon near the clock and choose **Open log folder**.
- **The log contains no dictated text** unless the Detailed log option has been turned on.

---

Hot Mic © 2026 Malcolm Syme. All rights reserved.
