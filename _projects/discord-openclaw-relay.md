---
layout: project
title: "Discord OpenClaw Relay"
description: "Practical LAN bridge that connects a Discord bot to OpenClaw Gateway across separate machines via WebSocket."
permalink: /discord-openclaw-relay/
github_url: "https://github.com/superdoccimo/discord-openclaw-relay"
image: /assets/logo.png
tags: ["Python", "Discord", "OpenClaw", "WebSocket", "LAN", "Self-Hosting"]
---

Discord OpenClaw Relay is a practical LAN bridge for real-world OpenClaw setups, connecting a Discord bot on one machine to OpenClaw Gateway on another via WebSocket.

**Architecture:**

```text
Host A (any machine)                   Host B (any machine)
┌─────────────────────┐                ┌──────────────────────────┐
│  python src/main.py │── WebSocket ──>│  OpenClaw Gateway        │
│  (Discord Bot)      │   LAN          │  ws://192.168.0.108:18789│
└─────────────────────┘                └──────────────────────────┘
```

**Key Features:**

- **Cross-host LAN deployment** — bot and OpenClaw run on separate machines (Linux, Windows, or any combination)
- **WebSocket relay** — communication over LAN, transparent to Discord users
- **Independent liveness** — if OpenClaw stops, the Discord bot stays logged in and returns status/error replies
- **Ed25519 device identity** — secure device pairing with OpenClaw Gateway
- **Long message splitting** — automatically splits AI responses exceeding Discord's 2000-char limit
- **Config separation** — all secrets in `.env` (gitignored), survives `git pull`

**Problems Solved:**

| Problem | Solution |
|---|---|
| Gateway binds to `127.0.0.1` only | LAN bind configuration guide included |
| Remote connection needs gateway token | `OPENCLAW_TOKEN` in `.env` |
| New device needs pairing approval | Ed25519 identity generation, one-time approval |
| Long AI responses exceed Discord limit | Auto-split on newline/space boundaries |
| `git pull` overwrites local config | All host-specific values in `.env` |

**Use Cases:**

For self-hosters running OpenClaw on a GPU box, homelab, or VPS who want their Discord bot on a separate machine. Fills the operational gaps not covered by OpenClaw's built-in same-host Discord integration.
