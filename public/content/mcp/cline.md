---
title: Pieces MCP + Cline Integration
path: /mcp/cline
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Cline lets you use Pieces Long-Term Memory in VS Code via the Cline extension, an AI coding agent that supports MCP.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Cline
metaDescription: Learn how to integrate Pieces MCP with Cline. Use SSE transport for reliable connection—Streamable HTTP has known compatibility issues.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/cline-mcp.png" alt="Pieces MCP integration with Cline" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Cline brings your workflow context directly into VS Code. Cline is an AI coding agent extension that maintains its own MCP configuration—it does **not** read from `.vscode/mcp.json`.

<Callout type="info">
  **Use SSE, not Streamable HTTP:** Cline has known compatibility issues with Streamable HTTP transport. Use the **SSE endpoint** for the most reliable connection.
</Callout>

## Prerequisites

There are **two** prerequisites for integrating Pieces with Cline as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up Cline

Cline stores its MCP configuration in a separate file: `~/.cline/data/settings/cline_mcp_settings.json`.

### Setup via Extension UI

<Steps>
  <Step title="Open VS Code">
    Open VS Code with the Cline extension installed.
  </Step>

  <Step title="Open Cline Settings">
    Click the `Cline` icon in the activity bar, then click the `gear icon` or navigate to **MCP Servers** in the Cline panel.
  </Step>

  <Step title="Add Server">
    Click `Add Server`, select **SSE** as the transport type, and enter:
    ```plaintext
    http://localhost:39300/model_context_protocol/2024-11-05/sse
    ```
  </Step>

  <Step title="Name the Server">
    Name it `pieces` and save.
  </Step>
</Steps>

### Manual JSON Config

Edit `~/.cline/data/settings/cline_mcp_settings.json`:

```json
{
  "mcpServers": {
    "pieces": {
      "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse",
      "type": "sse",
      "disabled": false,
      "autoApprove": []
    }
  }
}
```

### Auto-Approve Specific Tools

To skip confirmation prompts for specific Pieces tools:

```json
{
  "mcpServers": {
    "pieces": {
      "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse",
      "type": "sse",
      "autoApprove": ["ask_pieces_ltm", "workstream_summaries_full_text_search"]
    }
  }
}
```

## Using Pieces MCP Server in Cline

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Cline.

<Steps>
  <Step title="Open the Cline Panel">
    Open the Cline panel in VS Code.
  </Step>

  <Step title="Verify MCP Status">
    Check the **MCP** section for `pieces` with a connected status.
  </Step>

  <Step title="Use Agent Mode">
    Ensure Cline is in agent mode (not regular chat mode) so it can use MCP tools.
  </Step>

  <Step title="Begin Prompting">
    Ask Cline to search your LTM. For example: *"What was I working on yesterday?"*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit the config JSON and save. Cline reloads the server list from disk without requiring a VS Code restart.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Cline:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Cline Uses Its Own Config**: Cline reads from `~/.cline/data/settings/cline_mcp_settings.json`, not `.vscode/mcp.json`.

3. **Use SSE, Not Streamable HTTP**: Cline has compatibility issues with Streamable HTTP—use the SSE endpoint (`/model_context_protocol/2024-11-05/sse`).

4. **Use Agent Mode**: Ensure Cline is in agent mode, not regular chat mode.

5. **Server Disconnected**: Restart VS Code if the server shows as disconnected.

***

You're now set to enhance your Cline workflow with powerful context retrieval through Pieces MCP. Happy coding!
