---
title: Pieces MCP + Raycast Integration
path: /mcp/raycast
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Raycast lets you use Pieces Long-Term Memory in the Raycast macOS launcher via an stdio-to-HTTP bridge.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Raycast
metaDescription: Learn how to integrate Pieces MCP with Raycast. Raycast supports stdio only—use mcp-remote bridge to connect to PiecesOS. macOS only.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/raycast-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Raycast brings your workflow context directly into your macOS launcher. Raycast does not natively support HTTP-based MCP servers—you need an **stdio-to-HTTP bridge** (like [mcp-remote](/products/mcp/mcp-remote)) to connect to PiecesOS.

<Callout type="info">
  **macOS only:** Raycast is currently available only on macOS.
</Callout>

## Prerequisites

There are **three** prerequisites for integrating Pieces with Raycast:

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your workflow data.
  </Step>

  <Step title="Enable Long-Term Memory">
    Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>

  <Step title="Install Node.js">
    The `mcp-remote` bridge requires Node.js. Ensure Node.js and `npm` are installed.
  </Step>

  <Step title="Install mcp-remote">
    Install `mcp-remote` globally with a pinned version for security:

    ```bash
    npm install -g mcp-remote@0.1.38
    ```

    See [MCP Bridge](/products/mcp/mcp-remote) for why we recommend a locally installed binary over `npx`.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up Raycast

There are two ways to set up Pieces MCP for Raycast: use the Pieces CLI for automatic configuration, or configure manually with the mcp-remote bridge.

### Method 1: CLI Install (Recommended)

The Pieces CLI can automatically configure Pieces MCP for Raycast—no manual config editing required.

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
  <Step title="Select Raycast">
    A platform selection menu appears with options: *VS Code*, *Cursor*, *Claude Desktop*, *Windsurf*, *Claude Code*, *Raycast*, and *Warp*. Use the arrow keys to navigate to *Raycast*, then press `return` (macOS) or `enter` (Windows/Linux) to auto-install.
  </Step>
</Steps>

### Method 2: Manual Configuration with mcp-remote Bridge

Raycast uses `mcpServers` in its config. All servers must use `type: "stdio"` because Raycast does not support HTTP natively.

### Config File Location

Open Raycast, search for **Manage MCP Servers**, then press **Cmd+K** and select **Show Config File in Finder** to locate `mcp-config.json`.

### Local Setup (same machine as PiecesOS)

Add to `mcp-config.json`:

```json
{
  "mcpServers": {
    "pieces": {
      "command": "mcp-remote",
      "args": [
        "http://localhost:39300/model_context_protocol/2024-11-05/sse"
      ]
    }
  }
}
```

### Adding via Raycast UI

<Steps>
  <Step title="Open Raycast">
    Open Raycast (Cmd+Space or your hotkey) and search for **Install Server**.
  </Step>

  <Step title="Fill in the Form">
    * **Name:** pieces
    * **Type:** stdio
    * **Command:** mcp-remote
    * **Args:** `http://localhost:39300/model_context_protocol/2024-11-05/sse`
  </Step>
</Steps>

## Using Pieces MCP in Raycast

After setup, use `@pieces` in Raycast AI (Quick AI, AI Chat, or Presets) to invoke Pieces tools. Raycast automatically shows AI all available servers.

<Steps>
  <Step title="Open Raycast AI Chat">
    Open Raycast AI Chat.
  </Step>

  <Step title="Mention the Server">
    Type `@pieces` to mention the Pieces MCP server.
  </Step>

  <Step title="Ask Questions">
    Ask: *"What tools do you have from Pieces?"* or *"What was I working on yesterday?"*
  </Step>
</Steps>

## Updating

Edit `mcp-config.json` (found via **Show Config File in Finder**), update the URL in `args`, and restart Raycast AI.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Raycast:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **mcp-remote: command not found**: Run `npm install -g mcp-remote@0.1.38` and ensure the global npm bin directory is in your PATH.

3. **Bridge Not Connecting**: Verify the SSE endpoint responds: `curl http://localhost:39300/.well-known/version`

4. **Config File Location**: Use Raycast's **Manage MCP Servers > Show Config File in Finder** to locate the exact path.

***

You're now set to enhance your Raycast workflow with powerful context retrieval through Pieces MCP. Happy coding!
