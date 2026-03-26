---
title: Pieces MCP + Claude Code Integration
path: /mcp/claude-code
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Claude Code lets you use Pieces Long-Term Memory in the Claude Code CLI and VS Code extension via simple CLI commands.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Claude Code
metaDescription: Learn how to integrate Pieces MCP with Claude Code. Use the CLI to add Pieces LTM—automatically available in the VS Code extension.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/claude-code-mcp.png" alt="Pieces MCP integration with Claude Code" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Claude Code brings your workflow context directly into the Claude Code CLI and VS Code extension. Claude Code is Anthropic's developer-focused AI tool for coding tasks. Setup is simple: add Pieces via the CLI, and it's automatically available in the extension.

## Prerequisites

There are **two** prerequisites for integrating Pieces with Claude Code as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your workflow data.
  </Step>

  <Step title="Enable Long-Term Memory">
    Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up Claude Code

There are two ways to set up Pieces MCP for Claude Code: use the Pieces CLI for automatic configuration, or add the server manually via the Claude CLI.

### Method 1: CLI Install (Recommended)

The Pieces CLI can automatically configure Pieces MCP for Claude Code—no manual config editing required.

<Steps>
  <Step title="Install the Pieces CLI">
    Install the [Pieces CLI](/products/cli/get-started) if you haven't already.
  </Step>
  <Step title="Run the Setup Command">
    In your terminal, run:

    ```bash
    pieces mcp setup
    ```
  </Step>
  <Step title="Select Claude Code">
    A platform selection menu appears with options: *VS Code*, *Cursor*, *Claude Desktop*, *Windsurf*, *Claude Code*, *Raycast*, and *Warp*. Use the arrow keys to navigate to *Claude Code*, then press `return` (macOS) or `enter` (Windows/Linux) to auto-install.
  </Step>
</Steps>

### Method 2: Manual Setup via Claude CLI

Claude Code supports adding MCP servers via the CLI. Servers added via `claude mcp add` are automatically available in the Claude Code VS Code extension—no additional setup needed.

### Local Setup (Streamable HTTP — recommended)

Run in your terminal:

```bash
claude mcp add --transport http pieces http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

### Local Setup (SSE)

```bash
claude mcp add --transport sse pieces http://localhost:39300/model_context_protocol/2024-11-05/sse
```

### Project-Scoped Setup

To make Pieces MCP available only for the current project (stored in `.mcp.json` at project root):

```bash
claude mcp add --transport http --scope project pieces http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

### Managing Servers

```bash
# List all configured servers
claude mcp list

# Remove a server
claude mcp remove pieces

# Show server details
claude mcp get pieces
```

## Using Pieces MCP Server in Claude Code

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Claude Code.

<Steps>
  <Step title="Start a Session">
    Run `claude` in your terminal, or open a project in the Claude Code VS Code extension.
  </Step>

  <Step title="Verify Tools">
    Ask: *"What MCP tools do you have from Pieces?"* Pieces LTM tools should be listed.
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow. For example: *"What patterns did I use in my last React component?"* or *"Show me the authentication flow I implemented yesterday."*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

To update the URL, remove and re-add the server:

```bash
claude mcp remove pieces
claude mcp add --transport http pieces https://NEW_URL/model_context_protocol/2025-03-26/mcp
```

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Claude Code:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system. Test with: `curl http://localhost:39300/.well-known/version`

2. **Transport Error**: Try switching between `--transport http` and `--transport sse`.

3. **VS Code Extension Not Seeing Tools**: Restart VS Code after adding via CLI.

4. **Config Location**: User scope uses `~/.claude.json`; project scope uses `.mcp.json` at project root.

***

You're now set to enhance your Claude Code workflow with powerful context retrieval through Pieces MCP. Happy coding!
