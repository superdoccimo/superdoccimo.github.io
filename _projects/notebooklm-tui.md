---
layout: project
title: "NotebookLM TUI"
description: "A zero-dependency NotebookLM backup and restore toolkit for CLI and terminal UI workflows."
permalink: /notebooklm-tui/
github_url: "https://github.com/superdoccimo/notebooklm-tui"
image: /assets/logo.png
tags: ["Python", "CLI", "TUI", "NotebookLM", "Backup", "Google"]
---

NotebookLM TUI is a zero-dependency backup and restore toolkit for Google NotebookLM, providing both CLI tools and terminal UI workflows.

**Key Features:**

- **nlm-login:** Get NotebookLM auth cookies from your browser (Edge/Chrome/Brave/Firefox).
- **nlm-backup:** Download sources, artifacts, and notes from your notebooks.
- **nlm-upload:** Upload files/URLs and restore from backup folders.
- **nlm-tui / nlm-tui-en:** Interactive terminal UI in Japanese and English.
- **Zero Dependencies:** Core CLI and TUI tools run on Python standard library only.

**Technologies:**

- Python 3.10+
- Python standard library (no third-party packages)
- Cross-platform (Windows/Linux)
- Browser cookie integration (Edge/Chrome/Brave/Firefox)

**Quick Start:**

```bash
# Clone the repository
git clone https://github.com/superdoccimo/notebooklm-tui.git
cd notebooklm-tui

# Authenticate (opens your browser)
python nlm_login.py

# List notebooks
python nlm_backup.py --list

# Backup all notebooks
python nlm_backup.py --all
```

**Upload & Restore:**

```bash
# Upload files to a new notebook
python nlm_upload.py "My Research" paper.pdf notes.md

# Restore from a previous backup folder
python nlm_upload.py --restore ./downloads/My_Notebook/
```

**Use Cases:**

Perfect for users who want to back up their NotebookLM data, migrate notebooks, or manage NotebookLM content from the command line without installing any extra packages.
