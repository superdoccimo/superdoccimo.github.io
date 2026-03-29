---
layout: project
title: "Taskbar Click Fix"
description: "Windows 11 taskbar click fix tool using AutoHotkey v2 — observation logger and correction MVP for missed taskbar clicks."
permalink: /taskbar-click-fix/
github_url: "https://github.com/superdoccimo/taskbar-click-fix"
image: /assets/logo.png
tags: ["AutoHotkey", "Windows 11", "Taskbar", "Bug Fix", "MVP"]
---

Taskbar Click Fix is a Windows 11 taskbar click fix tool built with AutoHotkey v2, addressing the issue of missed or unresponsive taskbar clicks.

**Key Features:**

- **Observation Logger** (`taskbar_click_logger.ahk`) — records click duration, pointer movement, root window class, and foreground window changes to CSV
- **Correction MVP** (`taskbar_click_fix_mvp.ahk`) — detects short clicks on taskbar windows and injects a delayed button-up to ensure the click registers

**How the Correction Works:**

1. Watches left button down/up with `WH_MOUSE_LL`
2. Detects taskbar root windows (`Shell_TrayWnd`, `Shell_SecondaryTrayWnd`)
3. If button-up happens too quickly, swallows the original up event
4. Injects a delayed button-up so the effective hold reaches `MIN_HOLD_MS` (default: 40ms)

**Quick Start:**

1. Install AutoHotkey v2
2. Clone or copy the repository
3. Run `ahk/taskbar_click_logger.ahk` (observation) or `ahk/taskbar_click_fix_mvp.ahk` (correction)
4. Reproduce the taskbar click issue and inspect results

**Project Structure:**

- `ahk/taskbar_click_logger.ahk` — observation logger
- `ahk/taskbar_click_fix_mvp.ahk` — correction MVP
- `docs/research.md` — deep research report
- `docs/mvp-notes.md` — MVP scope and limitations
- `docs/quickstart-ja.md` — Japanese quickstart guide

**Use Cases:**

For Windows 11 users experiencing missed taskbar clicks, especially with Bluetooth mice or trackballs. Provides both diagnostic tools and an active fix.
