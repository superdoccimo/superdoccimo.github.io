---
layout: project
title: "WSL VHD Compact Utility"
description: "Utility scripts to compact the WSL VHD/VHDX file, featuring automatic detection, safe operation, read-only attachment, and automated Diskpart integration."
permalink: /vhdx/
github_url: "https://github.com/superdoccimo/VHDX"
image: /assets/logo.png
---

This repository provides utility scripts to compact the WSL (Windows Subsystem for Linux) VHD/VHDX file, which can grow over time. Two versions are available:

- **PowerShell Script**
- **Batch Script**

**Key Features:**

- **Automatic Detection:** Automatically locates the WSL VHD/VHDX file (e.g., `ext4.vhdx`) in common installation paths.
- **Safe Operation:** Checks if the VHD is already attached and detaches it if necessary.
- **Read-Only Attachment:** Attaches the VHD in read-only mode to ensure data integrity.
- **Automated Diskpart Integration:** Generates and executes a temporary Diskpart script to perform attach, compact, and detach operations.
- **Ease of Use:** Minimal configuration required—simply stop WSL and run the script with administrative privileges.

**Prerequisites:**

- **WSL Shutdown:** Run `wsl --shutdown` before executing the scripts.
- **Administrator Privileges:** The scripts must be run as an administrator.
- **Supported OS:** Windows systems running WSL.

**Usage:**

- **PowerShell Script:**  
  Open PowerShell as an administrator, navigate to the repository directory, and execute:
  ```powershell
  .\CompactWSLVHD.ps1
  ```
