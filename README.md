# Velvet — Windows test downloads

Velvet is a local AI chat app with spoken replies, custom personalities, and a portrait for each voice.

## Download

**[Download Velvet 1.2.0 for Windows (.exe)](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.2.0-test.1/Velvet-Setup-1.2.0-x64.exe)**

[Release notes](https://github.com/Xpomodz/velvet-downloads/releases/tag/v1.2.0-test.1) · [Installation guide](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.2.0-test.1/Velvet-Install-Guide.txt)

This is an **unsigned test prerelease**. Windows may show an unknown-publisher warning, and Smart App Control may block it. If blocked, keep Windows security enabled and send the developer a screenshot of the exact message.

## New in 1.2.0

- Native right-click editing and copying in text fields and chat replies.
- Improved personality setup with Llama 3.2 · 3B, the full Roger preset, an 8,000-character editor, and clear save status.
- A dark purple design with gradients across the app and setup screens.
- Changeable portraits that follow each voice in chat, the voice library, and the studio. PNG, JPEG, and WebP are supported, up to 8 MB.

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

[Verification report](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.2.0-test.1/Velvet-1.2.0-verification.json) · [SHA-256 checksums](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.2.0-test.1/SHA256SUMS.txt)

The application build and installer packaging passed, followed by 10 checks of the installed app's private runtime, editing roles, complete personality, portrait, actual CPU chat and speech, shutdown, and saved data after relaunch. Tests used an isolated runtime on the development PC; second-PC installation and Windows signing/trust acceptance remain unverified. See the release notes for the test scope.

This repository contains installers and supporting release documents. It does not contain the application's source code or private developer chat history. **Built with Llama.** Third-party and model license notices are included with the installer.
