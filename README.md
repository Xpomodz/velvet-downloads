# Velvet — Windows test downloads

Velvet is a local AI chat app with spoken replies, custom personalities, and a portrait for each voice.

## Download

**[Download Velvet 1.3.0 for Windows (.exe)](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.3.0-test.1/Velvet-Setup-1.3.0-x64.exe)**

[Release notes](https://github.com/Xpomodz/velvet-downloads/releases/tag/v1.3.0-test.1) · [Installation guide](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.3.0-test.1/Velvet-Install-Guide.txt)

This is an **unsigned test prerelease**. Windows may show an unknown-publisher warning, and Smart App Control may block it. If blocked, keep Windows security enabled and send the developer a screenshot of the exact message.

## New in 1.3.0

- Progress rings and bars for chat, speech and engine loading.
- Switch between chats, Voice studio and Settings while accepted jobs continue.
- One shared queue runs Velvet's heavy tasks one at a time, with visible queue positions and cancellation in **Activity**.
- Queued tasks retain the voice, model and personality selected when submitted. Completed output remains available after navigation and refresh.

Keep Velvet open while the queue works. Closing it stops unfinished work; completed conversations and recordings remain saved. Active cancellation can wait for the current model operation to finish. Speech percentages measure completed passages, not seconds remaining.

The purple gradients, native right-click editing, full Roger preset, 8,000-character personality editor and per-voice portraits from 1.2.0 remain available.

## Install or update

1. Close Velvet, download the installer, and open it.
2. Follow the installer. For an update, keep the existing installation location and use the same Windows account; no uninstall is needed. The local library and existing model selection are preserved.
3. Open Velvet and let first-time setup finish downloading the engines and models.

Requirements: **Windows 10 22H2 or Windows 11, Intel/AMD 64-bit, at least 16 GB RAM, and 30 GB free storage**. First setup needs internet. The chat model is approximately 2 GB; speech models, engines, and dependencies need several additional GB. CPU mode is available; NVIDIA graphics can accelerate processing.

## Make it yours

For an existing workspace, use **Settings → Use recommended model → Use Roger preset → Save preferences**. Skip **Use recommended model** if **Chat model** already shows **Llama 3.2 · 3B**. The model is selected only after it is downloaded and ready. Saved personality instructions apply to the next reply; character fidelity varies by model and prompt.

Select a voice, choose **Change portrait** in chat, pick an image, then choose **Save portrait**. You can also use **Add portrait / Change portrait** on its voice card. **Remove portrait** restores the orb in chat.

Normal chat, speech, dictation, and recordings are processed locally. First setup and additional downloads contact software/model download services. Your pictures and recordings remain on your computer.

## Verification

[Verification report](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.3.0-test.1/Velvet-1.3.0-verification.json) · [SHA-256 checksums](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.3.0-test.1/SHA256SUMS.txt)

The production build, 30 package-content checks, 70 backend tests, 23 desktop/installer tests, 9 controlled queue checks and 15 portrait/personality/layout regression checks passed. Seven checks of the installed app passed with real local CPU chat and speech, including queue order, navigation, cancellation, playback and persistence after restart.

Tests used an isolated private runtime on one Windows PC with cached downloads/models. Controlled browser engine adapters are identified separately in the report. Audio decoding and muted playback were verified; voice fidelity was not assessed. Second-PC installation, fresh downloads and Windows signing/trust acceptance remain unverified.

This repository contains installers and supporting release documents. It does not contain the application's source code or private developer chat history. **Built with Llama.** Third-party and model license notices are included with the installer.
