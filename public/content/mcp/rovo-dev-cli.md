---
title: Pieces MCP + Rovo Dev CLI Integration
path: /mcp/rovo-dev-cli
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Rovo Dev CLI (Atlassian's AI developer tool) lets you use Pieces Long-Term Memory directly from the command line.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Rovo Dev CLI
metaDescription: Learn how to integrate Pieces MCP with Rovo Dev CLI. Access Long-Term Memory for enhanced, context-aware productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/rovodevcli-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Rovo Dev CLI brings your workflow context directly into Atlassian's AI developer tool. Rovo Dev CLI supports stdio, SSE, and Streamable HTTP for flexible setup.

## Prerequisites

There are **two** prerequisites for integrating Pieces with Rovo Dev CLI as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up Rovo Dev CLI

Rovo Dev CLI stores its MCP configuration in `~/.rovodev/mcp.json`. It uses a `servers` root key with a `transport` field (not `type`).

### Config File Location

| Platform | Path |
|----------|------|
| **All platforms** | `~/.rovodev/mcp.json` |

### Local Setup (Streamable HTTP — recommended)

Edit `~/.rovodev/mcp.json`:

```json
{
  "servers": {
    "pieces": {
      "name": "Pieces LTM",
      "transport": "http",
      "url": "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
    }
  }
}
```

### Local Setup (SSE)

```json
{
  "servers": {
    "pieces": {
      "name": "Pieces LTM",
      "transport": "sse",
      "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse"
    }
  }
}
```

### Opening the Config in Your Editor

Run this command to open the config file in your default editor:

```bash
acli rovodev mcp
```

## Using Pieces MCP Server in Rovo Dev CLI

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Rovo Dev sessions.

<Steps>
  <Step title="Start a Rovo Dev Session">
    Start a Rovo Dev session from your terminal.
  </Step>

  <Step title="Check MCP Status">
    Run `/mcp list` to see configured servers and their status.
  </Step>

  <Step title="Begin Prompting">
    Ask: *"What Pieces tools do you have?"* or *"What was I working on yesterday?"*
  </Step>
</Steps>

### Managing Servers in Interactive Mode

Within a Rovo Dev session, use the `/mcp` command to open an interactive interface showing:

* Configured servers and their status
* Available tools from each server
* Enable/disable toggles

## Updating

Edit `~/.rovodev/mcp.json` (via `acli rovodev mcp` or directly), update the URL, and restart the Rovo Dev session.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Rovo Dev CLI:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Use transport, Not type**: Rovo Dev CLI uses the `transport` key (not `type`) for the transport type.

3. **Config File Not Found**: Create `~/.rovodev/` and `~/.rovodev/mcp.json` manually if the directory does not exist.

4. **Restart Session**: Restart the Rovo Dev session after editing the config.

5. **Atlassian OAuth**: Pieces does not require Atlassian OAuth. If prompted, this is for the Atlassian Rovo MCP Server, not Pieces.

***

You're now set to enhance your Rovo Dev CLI workflow with powerful context retrieval through Pieces MCP. Happy coding!
