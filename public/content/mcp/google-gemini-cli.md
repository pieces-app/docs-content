---
title: Pieces MCP + Google Gemini CLI Integration
path: /mcp/google-gemini-cli
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Google Gemini CLI lets you use Pieces Long-Term Memory directly from the Gemini command-line agent.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Google Gemini CLI
metaDescription: Learn how to integrate Pieces MCP with Google Gemini CLI. Use httpUrl for Streamable HTTP or url for SSE.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/google-gemini-mcp.png" alt="Pieces MCP integration with Google Gemini CLI" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Google Gemini CLI brings your workflow context directly into the Gemini command-line agent. Gemini CLI supports stdio, SSE, and Streamable HTTP.

<Callout type="info">
  **Key distinction:** For HTTP servers, use `httpUrl`; for SSE servers, use `url`—they are different fields in the Gemini config.
</Callout>

## Prerequisites

There are **two** prerequisites for integrating Pieces with Gemini CLI as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up Google Gemini CLI

Gemini CLI stores its MCP configuration in `~/.gemini/settings.json`. Workspace settings override user settings.

### Config File Location

| Scope | Path |
|-------|------|
| **User (global)** | `~/.gemini/settings.json` |
| **Workspace** | `YOUR_PROJECT/.gemini/settings.json` |

### Local Setup (Streamable HTTP — recommended)

Edit `~/.gemini/settings.json`:

```json
{
  "mcpServers": {
    "pieces": {
      "httpUrl": "http://localhost:39300/model_context_protocol/2025-03-26/mcp",
      "timeout": 30000
    }
  }
}
```

### Local Setup (SSE)

For SSE, use `url` instead of `httpUrl`:

```json
{
  "mcpServers": {
    "pieces": {
      "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse",
      "timeout": 30000
    }
  }
}
```

## Using Pieces MCP Server in Gemini CLI

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Gemini CLI.

<Steps>
  <Step title="Start a Gemini Session">
    Run `gemini` in your terminal.
  </Step>

  <Step title="Verify Tools">
    Gemini discovers and registers tools from MCP servers on startup. Ask: *"What Pieces tools are available?"*
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow.
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit `~/.gemini/settings.json`, update the URL, and start a new Gemini CLI session.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Gemini CLI:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **HTTP vs SSE Key**: Use `httpUrl` for Streamable HTTP, `url` for SSE—they are different fields.

3. **Settings File Not Found**: Create `~/.gemini/settings.json` manually.

4. **Tools Not Discovered**: Restart Gemini CLI after editing settings.

5. **OAuth Prompt**: Pieces does not require OAuth. Dismiss if prompted.

***

You're now set to enhance your Gemini CLI workflow with powerful context retrieval through Pieces MCP. Happy coding!
