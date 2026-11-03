# Velvet — Windows test downloads

Velvet is a local AI chat app with spoken replies, custom personalities, a portrait for each voice, and videos with timed captions.

## Download

**New: [Download Project Hub — the all-in-one installer](https://github.com/Xpomodz/project-hub-downloads/releases/download/v1.0.3/Project-Hub-Setup-1.0.3-x64.exe)** for Velvet, Sonora, Worktable, and PadForge. It detects existing apps and downloads only the tools you choose, with automatic updates per app. Internet access is required. [Project Hub release notes and files](https://github.com/Xpomodz/project-hub-downloads/releases/tag/v1.0.3).

**[Download Velvet 1.4.0 for Windows (.exe)](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.4.0-test.1/Velvet-Setup-1.4.0-x64.exe)**

[Release notes](https://github.com/Xpomodz/velvet-downloads/releases/tag/v1.4.0-test.1) · [Installation guide](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.4.0-test.1/Velvet-Install-Guide.txt)

This is an **unsigned test prerelease**. Windows may show an unknown-publisher warning, and Smart App Control may block it. If blocked, keep Windows security enabled and send the developer a screenshot of the exact message.

## New in 1.4.0

- Attach a video and choose its existing audio, a saved Velvet recording, or imported audio.
- **TikTok Hype** captions: bold uppercase white text, black outline, a yellow highlight following the spoken word, and a brief pop.
- Play, seek or expand the preview; correct recognized words while keeping their timings; export a captioned **MP4** or a separate **SRT**.
- **Use in video** in Voice studio preselects a recording. Saved projects keep their soundtrack, captions and exports after reopening Velvet.
- Video processing and export join the existing one-at-a-time **Activity** queue, so you can switch to chats and Voice studio while they work.

Open **Video captions → New video** to start. Videos may be MP4, MOV, M4V or WebM, up to 500 MB and five minutes; imported audio may be up to 200 MB. Recognition currently uses English. Replacement audio starts at zero, trims to the video length or pads with silence. Review the words before export.

Keep Velvet open while the queue works. Closing it stops unfinished work; completed chats, recordings and video projects remain saved. Cancellation waits for the current native operation to return. The purple design, progress indicators, native right-click editing, full Roger preset and per-voice portraits remain available.

## Install or update

1. Close Velvet, download the installer, and open it.
2. Follow the installer. For an update, keep the existing installation location and use the same Windows account; no uninstall is needed. The local library and existing model selection are preserved.
3. Open Velvet and let first-time setup finish downloading the engines and models.

Requirements: **Windows 10 22H2 or Windows 11, Intel/AMD 64-bit, at least 16 GB RAM, and 30 GB free storage**. First setup needs internet. The chat model is approximately 2 GB; speech models, engines, and dependencies need several additional GB. CPU mode is available; NVIDIA graphics can accelerate processing.

## Make it yours

For an existing workspace, use **Settings → Use recommended model → Use Roger preset → Save preferences**. Skip **Use recommended model** if **Chat model** already shows **Llama 3.2 · 3B**. The model is selected only after it is downloaded and ready. Saved personality instructions apply to the next reply; character fidelity varies by model and prompt.

Select a voice, choose **Change portrait** in chat, pick an image, then choose **Save portrait**. You can also use **Add portrait / Change portrait** on its voice card. **Remove portrait** restores the orb in chat.

Normal chat, speech, dictation, video captions and exports are processed locally. First setup and additional downloads contact software/model download services. Your pictures and recordings remain on your computer.

## Verification

[Verification report](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.4.0-test.1/Velvet-1.4.0-verification.json) · [SHA-256 checksums](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.4.0-test.1/SHA256SUMS.txt)

The production build, 41 package-content checks, 115 backend tests, 23 desktop/installer tests, 12 caption-browser checks, 9 queue checks and 16 feedback checks passed. Four checks of the actual installed app passed using real local CPU Whisper, actual MP4/SRT downloads and saved-project persistence after app restart. Exported audio, video frames and timed word highlights were checked independently.

Tests used an isolated private runtime on one Windows PC with seeded downloads/models. The controlled caption-browser suite replaces only word recognition; the separate installed run recognizes one short English speech sample with the real engine. Physical speaker output, general recognition accuracy, second-PC installation, fresh network setup and Windows signing/trust acceptance remain unverified.

This repository contains installers and supporting release documents. It does not contain the application's source code or private developer chat history. **Built with Llama.** Third-party and model license notices are included with the installer.
