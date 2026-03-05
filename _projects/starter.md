---
layout: project
title: "Tech-over-Gold Starter"
description: "Evidence scorecard CLI + content templates + JSON-LD. A pragmatic starter to turn ideas into repeatable tools."
permalink: /starter/
github_url: "https://github.com/superdoccimo/starter"
image: /assets/logo.png
tags: ["Python", "CLI", "JSON-LD", "SEO", "ChatGPT", "Codex"]
---

Tech-over-Gold Starter is a pragmatic starter kit to turn ideas into repeatable tools, built with assistance from ChatGPT and Codex.

**Key Features:**

- **Evidence Scorecard (CLI):** Score posts and articles by provenance and reproducibility.
- **Content Templates:** YouTube/Blog templates with JSON-LD support (Article/FAQ/Breadcrumb).
- **Decision Checklists:** Condition tables for allocation switching from gold to technology.
- **Roadmap:** Manual to semi-automation path (WordPress/Strapi/Next.js/Sheets).

**Technologies:**

- Python
- JSON-LD (Article, FAQ, Breadcrumb)
- ChatGPT / Codex assisted development

**Quick Start:**

```bash
python3 scripts/scorecard_cli.py \
  --title "Example claim" \
  --source-type social \
  --provenance unknown \
  --independent-corroboration 1 \
  --reply-behavior ignores_questions
```

**Project Structure:**

- `scripts/scorecard_cli.py` — CLI scoring tool
- `templates/` — YouTube & Blog templates + JSON-LD
- `docs/ROADMAP.md` — Milestones and expansion plans
- `data/indicators.schema.json` — Schema for signals

**Use Cases:**

Ideal for content creators and researchers who want to evaluate the credibility of claims using a structured, reproducible scoring methodology. Combines evidence-based analysis with SEO-ready content templates.
