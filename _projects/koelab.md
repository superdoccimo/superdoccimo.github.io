---
layout: project
title: "koelab"
description: "Ollama for Voice — a local voice conversion and TTS workbench unifying voice conversion, Japanese/multilingual TTS, WebUI, and real-time CLI workflows."
permalink: /koelab/
github_url: "https://github.com/superdoccimo/koelab"
image: /assets/logo.png
tags: ["Python", "Voice Conversion", "TTS", "CLI", "WebUI", "Docker", "Local AI"]
---

koelab is a local voice conversion and TTS workbench — "Ollama for Voice" — unifying voice conversion, Japanese TTS, multilingual TTS, WebUI workflows, and real-time CLI workflows in one project.

**Key Features:**

- **Voice Conversion** — convert source audio using a target reference voice
- **Japanese & Multilingual TTS** — synthesize speech from text with multiple model backends
- **Real-Time CLI Workflows** — live voice conversion from microphone input
- **WebUI + REST API** — browser-based interface and programmatic access
- **Model Registry** — pull, list, search, and inspect models with simple commands
- **Local-First** — practical local alternative to hosted services for control, privacy, and hackability
- **Docker Support** — containerized deployment with `docker compose`

**Quick Start:**

```bash
pip install koelab

# Pull a voice model
koelab pull seed-vc

# Convert voice
koelab run seed-vc --input source.wav --reference target_voice.wav --output converted.wav
```

**Core Commands:**

| Command | Description |
|---------|-------------|
| `koelab pull <model>` | Download a voice model |
| `koelab run <model>` | Run voice conversion |
| `koelab speak <model>` | Synthesize speech from text |
| `koelab live <model>` | Real-time voice conversion from mic |
| `koelab serve` | Start REST API server + WebUI |
| `koelab doctor` | Inspect runtime dependencies and setup problems |
| `koelab models` | Show all available models from registry |

**Technologies:**

- Python 3.11+ (3.12 recommended)
- Voice conversion models (seed-vc, etc.)
- TTS backends (Irodori-TTS, XTTS-v2)
- FFmpeg integration (recommended via [autoffmpeg](https://github.com/superdoccimo/autoffmpeg))
- Docker / docker compose

**Use Cases:**

For developers and creators who want a local, hackable alternative to hosted voice services. Ideal for voice conversion experiments, multilingual TTS workflows, real-time voice transformation, and privacy-conscious audio processing.
