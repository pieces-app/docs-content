---
title: Pieces MCP + Windsurf Integration
path: /mcp/windsurf
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Windsurf lets you use Pieces Long-Term Memory directly in the Windsurf IDE, enhancing your coding workflow with context-aware AI assistance via Cascade.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Windsurf
metaDescription: Learn how to integrate Pieces MCP with Windsurf. Access Long-Term Memory within Cascade for enhanced, context-aware productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/windsurf-mcp.png" alt="Pieces MCP integration with Windsurf" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Windsurf brings your workflow context directly into the Cascade AI panel. With this integration, Windsurf can access your past work, similar code, and historical debugging context to provide smarter, personalized assistance.

## Prerequisites

There are **two** prerequisites for integrating Pieces with Windsurf as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your workflow data and pass context through to Windsurf.

    If you do not have PiecesOS, you can download it alongside the [Pieces Desktop App](/products/desktop/download) or [install it standalone](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation) here.
  </Step>

  <Step title="Enable Long-Term Memory">
    For the MCP server to interact with your workflow context, you must enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

### Getting the MCP Endpoint for PiecesOS

To use Pieces MCP with Windsurf, you'll need the MCP endpoint from PiecesOS:

```plaintext
http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

<Callout type="alert">
  Keep in mind that the **specific port** (e.g., `39300`) PiecesOS is running on **may vary**.
</Callout>

<Callout type="info">
  Windsurf uses **`serverUrl`** (not `url`) for HTTP/remote servers—this is a Windsurf-specific key name.
</Callout>

## Setting Up Windsurf

There are two ways to set up Pieces MCP for Windsurf: use the Pieces CLI for automatic configuration, or configure manually.

### Method 1: CLI Install (Recommended)

The Pieces CLI can automatically configure Pieces MCP for Windsurf—no manual config editing required.

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
  <Step title="Select Windsurf">
    A platform selection menu appears with options: *VS Code*, *Cursor*, *Claude Desktop*, *Windsurf*, *Claude Code*, *Raycast*, and *Warp*. Use the arrow keys to navigate to *Windsurf*, then press `return` (macOS) or `enter` (Windows/Linux) to auto-install.
  </Step>
</Steps>

### Method 2: Manual Configuration

Windsurf stores its MCP configuration in a global config file. Edit `~/.codeium/windsurf/mcp_config.json`:

### Local Setup (Streamable HTTP — recommended)

```json
{
  "mcpServers": {
    "pieces": {
      "serverUrl": "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
    }
  }
}
```

### Adding via MCP Marketplace

<Steps>
  <Step title="Open the Cascade Panel">
    Open the Cascade panel in Windsurf.
  </Step>

  <Step title="Open the MCP Marketplace">
    Click the `MCP icon` to open the MCP Marketplace.
  </Step>

  <Step title="Add Pieces">
    Search for Pieces, or click `Add custom` and enter your MCP URL.
  </Step>
</Steps>

## Using Pieces MCP Server in Windsurf

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Windsurf through the Cascade panel.

<Steps>
  <Step title="Open the Cascade Panel">
    Open the Cascade AI panel in Windsurf.
  </Step>

  <Step title="Verify MCP Tools">
    Check the MCP tools section—Pieces LTM tools should appear. Ask Cascade: *"What Pieces tools are available?"*
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow. For example: *"What was I working on yesterday?"* or *"Show me similar code snippets to this React component."*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit `~/.codeium/windsurf/mcp_config.json`, update the `serverUrl`, then restart Windsurf.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Windsurf:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Confirm LTM Engine Activation**: Make sure the [Long-Term Memory Engine (LTM-2.7) is enabled in PiecesOS](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine).

3. **Use serverUrl, Not url**: Windsurf requires the `serverUrl` key—using `url` will not work.

4. **Restart Windsurf**: After editing `mcp_config.json`, restart Windsurf for changes to take effect.

5. **Disable a Server**: Add `"disabled": true` to the server config object if you need to temporarily disable Pieces MCP.

***

You're now set to enhance your Windsurf workflow with powerful context retrieval through Pieces MCP. Happy coding!
