---
title: Pieces MCP + Amazon Q Developer Integration
path: /mcp/amazon-q-developer
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Amazon Q Developer lets you use Pieces Long-Term Memory in the Amazon Q CLI and IDE plugin for enhanced, context-aware productivity.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Amazon Q Developer
metaDescription: Learn how to integrate Pieces MCP with Amazon Q Developer. Access Long-Term Memory in CLI and IDE for enhanced productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/amazon-q-dev-mcp.png" alt="Pieces MCP integration with Amazon Q Developer" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Amazon Q Developer brings your workflow context directly into AWS's AI assistant, available both as a CLI and an IDE plugin. You can ask Q about past implementations, similar code, and historical debugging context.

## Prerequisites

There are **two** prerequisites for integrating Pieces with Amazon Q as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up Amazon Q Developer

Amazon Q supports both IDE plugin and CLI configurations. The IDE uses `~/.aws/amazonq/default.json` (or the legacy `mcp.json`). Workspace settings take precedence over global settings.

### IDE Plugin Setup (Local)

Edit `~/.aws/amazonq/default.json`:

```json
{
  "servers": {
    "pieces": {
      "type": "http",
      "url": "http://localhost:39300/model_context_protocol/2025-03-26/mcp",
      "timeout": 60
    }
  }
}
```

### CLI Setup

Configure the MCP server in the CLI:

```bash
q mcp add --name pieces --type http --url http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

### Tool Permissions

Amazon Q allows per-tool permission levels. You can configure these in the IDE settings UI after adding the server:

* **Ask** — prompts before each use
* **Always allow** — runs without prompting
* **Deny** — blocked entirely

## Using Pieces MCP Server in Amazon Q

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Amazon Q.

<Steps>
  <Step title="Start Amazon Q">
    Start Amazon Q (CLI or IDE).
  </Step>

  <Step title="Verify MCP Loading">
    MCP servers load in the background; tools become available progressively.
  </Step>

  <Step title="Begin Prompting">
    Ask Q: *"What Pieces tools are available?"* or *"What was I working on yesterday?"*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit `~/.aws/amazonq/default.json`, update the `url`, and restart Amazon Q or start a new session.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Amazon Q Developer:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Config Directory Doesn't Exist**: Create `~/.aws/amazonq/` manually.

3. **Legacy vs Current Config**: Both `default.json` and `mcp.json` are supported; `default.json` takes precedence.

4. **MCP Not Loading**: Ensure you have a recent version of Amazon Q Developer.

5. **OAuth Prompt**: Pieces does not require OAuth. Use no-auth configuration.

***

You're now set to enhance your Amazon Q Developer workflow with powerful context retrieval through Pieces MCP. Happy coding!
