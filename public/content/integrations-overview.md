---
title: Integrations Overview
path: /integrations-overview
visibility: PUBLIC
status: PUBLISHED
description: Choose how to connect Pieces to your development workflow - MCP Server for AI-powered IDEs or CLI for terminal-based development.
metaTitle: Integrations Overview | Connect Pieces to Your Workflow
metaDescription: Discover how to integrate Pieces with your development tools via MCP Server or CLI. Learn which integration fits your workflow best.
---

## Connecting Pieces to Your Workflow

Pieces integrates with your development environment in two powerful ways: **MCP Server** for AI-powered IDE integrations, or **CLI** for terminal-based workflows. Both connect to [PiecesOS](/products/core-dependencies/pieces-os) to provide access to your [Long-Term Memory](/products/desktop/long-term-memory) and [Timeline](/products/desktop/timeline)—the primary surfaces for captured workflow context. [Pieces Drive](/products/desktop/drive) remains available as a **legacy** material manager for existing saved snippets; new workflows should rely on LTM and Timeline instead.

## Choosing Your Integration

### MCP Server (Recommended for AI-Powered Development)

The **Model Context Protocol (MCP) Server** connects AI assistants like Claude, GitHub Copilot, and Cursor directly to your Pieces Long-Term Memory. MCP enables your AI coding assistants to understand your workflow context, past decisions, and project history.

**Best for:**
- AI-assisted coding in IDEs (Cursor, VS Code, JetBrains)
- Context-aware AI conversations
- Teams using AI coding assistants
- Visual development workflows

**Supported clients:**
- Cursor, VS Code, GitHub Copilot
- Claude Desktop, Claude Code
- JetBrains IDEs (IntelliJ, PyCharm, WebStorm)
- Windsurf, Cline, Continue.dev, Zed
- And 15+ more AI-powered tools

<FancyCard title="MCP Server" href="/products/mcp" colored={false}>
  Connect AI assistants to your Pieces Long-Term Memory with Model Context Protocol integration.
</FancyCard>

***

### CLI (Command-Line Interface)

The **Pieces CLI** brings Pieces functionality to your terminal with commands for saving snippets, querying your Long-Term Memory, and accessing Conversational Search from the command line.

**Best for:**
- Terminal-based development workflows
- Command-line power users
- Scripting and automation
- Headless environments

**Key features:**
- Conversational Search from your terminal
- Legacy [Pieces Drive](/products/cli/drive) commands in the CLI (save, search, share materials) for users who still rely on Drive
- Terminal UI (TUI) for visual navigation
- Long-Term Memory queries from CLI

<FancyCard title="CLI" href="/products/cli" colored={false}>
  Access Pieces features directly from your terminal with the command-line interface.
</FancyCard>

***

## Decision Guide

### Choose MCP Server if you:
- Use AI coding assistants (Claude, GitHub Copilot, Cursor)
- Work primarily in IDEs or code editors
- Want AI to understand your workflow history
- Need context-aware code suggestions

### Choose CLI if you:
- Prefer terminal-based workflows
- Write scripts or automation
- Work in headless or remote environments
- Want quick snippet management from command line

### Use Both!
Many developers use **both** integrations:
- MCP for AI-assisted coding in their IDE
- CLI for quick terminal operations and scripting

***

## Prerequisites

Both integrations require:

1. **[PiecesOS](/products/core-dependencies/pieces-os)** installed and running
2. **[Long-Term Memory enabled](/products/meet-pieces/enabling-long-term-memory)** (for context-aware features)
3. Your development tools installed (IDEs, terminal, etc.)

***

## Quick Start

### MCP Server Setup

<Steps>
  <Step title="Install PiecesOS">
    [Download and install PiecesOS](/products/core-dependencies/pieces-os/manual-installation) for your platform (macOS, Windows, Linux).
  </Step>

  <Step title="Enable Long-Term Memory">
    Open Pieces Desktop and [enable Long-Term Memory](/products/meet-pieces/enabling-long-term-memory) to start capturing workflow context.
  </Step>

  <Step title="Choose Your Client">
    Select your AI tool or IDE from the [MCP integrations list](/products/mcp) and follow the setup guide.
  </Step>
</Steps>

***

### CLI Setup

<Steps>
  <Step title="Install PiecesOS">
    [Download and install PiecesOS](/products/core-dependencies/pieces-os/manual-installation) for your platform.
  </Step>

  <Step title="Install Pieces CLI">
    Follow the [CLI installation guide](/products/cli/get-started) to install the command-line tool.
  </Step>

  <Step title="Start Using CLI">
    Run `pieces` commands in your terminal or launch the [TUI](/products/cli/tui) with `pieces tui`.
  </Step>
</Steps>

***

## Next Steps

Ready to connect Pieces to your workflow?

<FancyCard title="MCP Server Documentation" href="/products/mcp" colored={false}>
  Learn about Model Context Protocol and browse 20+ supported AI clients and IDEs.
</FancyCard>

<FancyCard title="CLI Documentation" href="/products/cli" colored={false}>
  Explore CLI commands, Conversational Search, legacy Drive workflows, and Terminal UI features.
</FancyCard>

***

## Need Help?

Visit [Support](/products/support) for troubleshooting guides, FAQs, and community resources.
