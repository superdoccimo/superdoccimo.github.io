---
layout: project
title: "Gemini 72h Visibility"
description: "Documentation of Google Gemini's up-to-72-hour data retention even when activity tracking is turned off, based on official sources."
permalink: /gemini-72h-visibility/
github_url: "https://github.com/superdoccimo/gemini-72h-visibility"
image: /assets/logo.png
tags: ["Privacy", "Google Gemini", "GDPR", "Data Retention", "Documentation"]
---

This repository documents, using official Google documentation, that turning Gemini Apps Activity OFF may still allow conversations to be saved for up to 72 hours — and that this short-term retention does not appear in Gemini Apps Activity.

**Key Points:**

- **Keep Activity OFF does not mean immediate zero retention** — conversations may still be saved for up to 72 hours.
- **Invisible retention** — this short-term data does not appear in your Gemini Apps Activity history.
- **Official sources only** — all findings are based on Google's own published documentation.
- **GDPR relevance** — raises questions about transparency under EU data protection regulations.

**Primary Sources:**

| Source | Key Quote |
|--------|-----------|
| [Manage & delete your Gemini Apps activity](https://support.google.com/gemini/answer/13278892?hl=en) | "Even when Keep Activity is off, ... saved ... up to 72 hours ... won't appear in your Gemini Apps Activity." |
| [Google Workspace Updates Blog](https://workspaceupdates.googleblog.com/2025/05/pre-configure-the-gemini-app-conversation-history-admin-setting.html) | Conversation history OFF still allows up to 72-hour retention |

**Why It Matters:**

- **Expectation gap** — users commonly interpret "OFF" as "not saved at all"
- **No user audit** — short-term retention is not visible in Activity logs
- **Consumer vs Enterprise** — Workspace/Cloud users get stronger privacy guarantees; individual users do not

**Practical Guidance:**

- Do not paste secrets, PII, credentials, or API keys into Gemini
- Understand that up to 72 hours of retention may still occur even with Activity OFF
- Consider local archiving if you need conversation history
- Review Workspace/Cloud data governance options if applicable
