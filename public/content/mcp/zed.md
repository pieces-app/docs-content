---
title: Pieces MCP + Zed Integration
path: /mcp/zed
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Zed lets you use Pieces Long-Term Memory in the Zed editor using an stdio-to-HTTP bridge, enhancing your coding workflow with context-aware AI assistance.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Zed
metaDescription: Learn how to integrate Pieces MCP with Zed. Zed uses stdio only—connect via mcp-remote bridge to access Long-Term Memory.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/zed-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Zed brings your workflow context directly into the Zed editor. Because Zed currently supports **stdio only** (not native HTTP), you'll use an stdio-to-HTTP bridge such as [mcp-remote](/products/mcp/mcp-remote) to connect to PiecesOS.

## Prerequisites

There are **three** prerequisites for integrating Pieces with Zed:

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

## Setting Up Zed with mcp-remote Bridge

Zed uses a custom `context_servers` key (not `mcpServers` or `servers`). Because Zed does not support HTTP MCP servers natively, you must use the `mcp-remote` bridge.

### Config File Location

| Scope | Path |
|-------|------|
| **User settings** | `~/.config/zed/settings.json` (Linux/macOS) |
| **Project settings** | `.zed/settings.json` in your project root |

### Local Setup (same machine as PiecesOS)

Add to `~/.config/zed/settings.json`:

```json
{
  "context_servers": {
    "pieces": {
      "command": {
        "path": "mcp-remote",
        "args": [
          "http://localhost:39300/model_context_protocol/2024-11-05/sse"
        ],
        "env": {}
      },
      "settings": {}
    }
  }
}
```

<Callout type="alert">
  The port (e.g., `39300`) may vary. Find your current PiecesOS port in the PiecesOS Quick Menu under **Model Context Protocol (MCP) Servers**.
</Callout>

### Alternative: supergateway Bridge

You can also use `supergateway` instead of `mcp-remote`. Install with `npm install -g supergateway`, then use `"path": "supergateway"` and `"args": ["--sse", "http://localhost:39300/model_context_protocol/2024-11-05/sse"]`. For security, prefer a locally installed binary over `npx`.

## Using Pieces MCP Server in Zed

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Zed's AI assistant panel.

<Steps>
  <Step title="Open Zed's AI Assistant Panel">
    Open the AI assistant panel in Zed.
  </Step>

  <Step title="Verify Tools">
    Ask: *"What context tools do you have?"* Pieces LTM tools should be available.
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow, such as: *"What was I working on yesterday?"*
  </Step>
</Steps>

## Updating

Edit your `settings.json`, update the URL in the `args` array, and save. Zed reloads context servers on config change.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Zed:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Use context_servers**: Zed uses `context_servers`, not `mcpServers` or `servers`.

3. **mcp-remote: command not found**: Run `npm install -g mcp-remote@0.1.38` and ensure the global npm bin directory is in your PATH.

4. **Bridge process crashes**: Check that PiecesOS is running and the SSE endpoint responds. You can test with: `curl http://localhost:39300/.well-known/version`

5. **No tools visible**: Restart Zed; ensure `mcp-remote` is in your PATH.

***

You're now set to enhance your Zed workflow with powerful context retrieval through Pieces MCP. Happy coding!
