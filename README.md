# Velvet — Windows test downloads

Velvet is a local AI chat app with spoken replies.

## Download

**[Download Velvet 1.1.1 for Windows (143 MB)](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.1.1-test.1/Velvet-Setup-1.1.1-x64.exe)**

[Release notes and verification files](https://github.com/Xpomodz/velvet-downloads/releases/tag/v1.1.1-test.1) · [Installation guide](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.1.1-test.1/Velvet-Install-Guide.txt) · [Checksums](https://github.com/Xpomodz/velvet-downloads/releases/download/v1.1.1-test.1/SHA256SUMS.txt)

This is an **unsigned test build**. Windows may show an unknown-publisher warning, and Smart App Control may block it. If blocked, send the developer a screenshot of the exact message and keep Windows security enabled.

## Install

1. Download `Velvet-Setup-1.1.1-x64.exe` and open it.
2. Follow the installer, then let Velvet download its local engines and models.
3. Open Velvet and send a short message to test chat and the spoken reply.

First setup needs internet and downloads several GB. Requirements: Windows 10 22H2 or Windows 11 on Intel/AMD 64-bit, at least 16 GB RAM, and 30 GB free storage. An NVIDIA GPU is helpful; CPU mode is available and slower.

## Verification

Version 1.1.1 passed 13 installer tests and 25 backend tests. The installed app was checked for private runtime setup, actual CPU chat and automatic speech, shutdown, and saved conversation/settings after relaunch.

These checks used an isolated runtime on the development PC and reused downloaded caches. Installation on a separate PC and Windows trust/signing acceptance remain unverified.

Installer SHA-256:

```text
a72d2097e18569ecfae37ff3fe533b88d90f157d2d5500c294930264dde8e43b
```

This repository contains test installers and supporting release documents. It does not contain the application's source code or private chat history.
