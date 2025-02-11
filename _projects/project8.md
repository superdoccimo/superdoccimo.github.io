---
layout: project
title: "FFmpeg Automatic Installation Script"
description: "A PowerShell script that automates downloading, extracting, and installing FFmpeg on Windows, including environment variable setup and safe reinstallation."
permalink: /autoffmpeg/
github_url: "https://github.com/superdoccimo/autoffmpeg"
---

This project provides a PowerShell script that automates the entire FFmpeg installation process on Windows systems. The script handles:

- **Downloading:** Automatically fetches the latest FFmpeg builds from the official BtbN releases.
- **Extraction & Installation:** Unpacks the downloaded files and installs FFmpeg.
- **Environment Variable Setup:** Configures the necessary PATH variables for FFmpeg.
- **Reinstallation:** Safely removes any existing FFmpeg installation before updating to the latest version.
- **Status Feedback:** Provides clear status messages during installation and verifies success.

**Requirements:**

- Windows 10/11
- PowerShell (run as Administrator)
- An active Internet connection

**Usage:**

1. Save the script as `install_ffmpeg.ps1`.
2. Open PowerShell as Administrator and, if necessary, bypass the execution policy:
   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
