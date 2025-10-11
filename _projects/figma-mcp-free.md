---
layout: project
title: "Figma MCP Free"
description: "Open-source alternative to Figma's paid Dev Mode - Free MCP server with read-only access to Figma's REST API"
permalink: /figma-mcp-free/
github_url: "https://github.com/superdoccimo/figma-mcp-free"
image: /assets/logo.png
tags: ["TypeScript", "Figma", "MCP", "Design Tokens", "React", "Vue", "Svelte"]
---

Figma MCP Free is an open-source alternative to Figma's paid Dev Mode, providing a free MCP (Manifest Component Protocol) server with read-only access to Figma's REST API.

**Key Features:**

- **Design Token Extraction:** Export design tokens in W3C format from Figma files.
- **Component Discovery:** List and query design components with CLI tools.
- **Multi-Framework Code Generation:** Generate code for React, Vue, Svelte, and HTML.
- **Read-Only API Access:** Safe, non-destructive operations using Personal Access Token.
- **Free & Open Source:** Community-driven alternative to monetized solutions.

**Technologies:**

- TypeScript
- Figma REST API
- MCP (Manifest Component Protocol)
- React, Vue, Svelte support
- pnpm workspace

**Installation:**

```bash
# Clone and install
git clone https://github.com/superdoccimo/figma-mcp-free.git
cd figma-mcp-free
pnpm install && pnpm -r build

# Initialize with your Figma token
pnpm --filter figma-mcp-free dev -- init
```

**Quick Start:**

```bash
# Find components in a Figma file
pnpm --filter figma-mcp-free dev -- components <FILE_ID>

# Generate code for a component
pnpm --filter figma-mcp-free dev -- generate <FILE_ID> <NODE_ID> --framework react
```

**Use Cases:**

Perfect for developers who need to extract design tokens and generate code from Figma designs without paying for Dev Mode. Ideal for indie developers, open-source projects, and teams looking for cost-effective design-to-code workflows with full transparency and control.
