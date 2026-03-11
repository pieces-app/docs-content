---
title: Pieces MCP + VS Code Integration
path: /mcp/vs-code
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Visual Studio Code lets you use Pieces Long-Term Memory directly in your editor, enhancing your coding workflow with context-aware AI assistance.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with VS Code
metaDescription: Learn how to integrate Pieces MCP with Visual Studio Code. Access Long-Term Memory within your editor for enhanced, context-aware productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/visual-studio-code-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Visual Studio Code brings your workflow context directly into your editor. With this integration, your AI assistant can access past implementations, similar code, and historical debugging context—without searching through commits or notes.

## Prerequisites

There are **two** prerequisites for integrating Pieces with VS Code as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your workflow data and pass context through to VS Code.

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

To use Pieces MCP with VS Code, you'll need the MCP endpoint from PiecesOS. VS Code supports Streamable HTTP (recommended) or SSE.

**Streamable HTTP (recommended):**
```plaintext
http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

**SSE (legacy):**
```plaintext
http://localhost:39300/model_context_protocol/2024-11-05/sse
```

<Callout type="alert">
  Keep in mind that the **specific port** (e.g., `39300`) PiecesOS is running on **may vary**.
</Callout>

To find the current MCP endpoint with the active instance of PiecesOS, open the PiecesOS Quick Menu and expand the **Model Context Protocol (MCP) Servers** tab. You can copy the endpoint, which includes the active port number.

You can also find this in the Pieces Desktop App by opening **Settings** and clicking **Model Context Protocol (MCP)**.

## Setting Up VS Code

There are two ways to set up Pieces MCP for VS Code: use the Pieces CLI for automatic configuration, or configure manually.

### One-Click Install

Install Pieces MCP in VS Code with a single click. Ensure [PiecesOS is running](/products/core-dependencies/pieces-os) and [Long-Term Memory is enabled](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine) before clicking.

<mcp-install-badges platforms="vscode" />

### Method 1: CLI Install (Recommended)

The Pieces CLI can automatically configure Pieces MCP for VS Code—no manual config editing required.

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
  <Step title="Select VS Code">
    A platform selection menu appears with options: *VS Code*, *Cursor*, *Claude Desktop*, *Windsurf*, *Claude Code*, *Raycast*, and *Warp*. Use the arrow keys to navigate to *VS Code*, then press `return` (macOS) or `enter` (Windows/Linux) to auto-install.
  </Step>
  <Step title="Choose Scope (if prompted)">
    For VS Code, you'll be asked to choose *User Settings* (MCP available in all projects) or *Workspace Settings* (MCP for the current project only).
  </Step>
</Steps>

### Method 2: Manual Configuration

VS Code uses a `servers` root key (not `mcpServers`) in its MCP configuration. The transport type is set with a `type` field.

### Config File Location

| Scope | Path |
|-------|------|
| **Workspace** | `.vscode/mcp.json` in your project root |
| **User (global)** | Via Settings > search "MCP Servers" |

### Local Setup (Streamable HTTP — recommended)

Add or edit `.vscode/mcp.json` in your project root:

```json
{
  "servers": {
    "pieces": {
      "type": "http",
      "url": "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
    }
  }
}
```

### Local Setup (SSE — legacy)

```json
{
  "servers": {
    "pieces": {
      "type": "sse",
      "url": "http://localhost:39300/model_context_protocol/2024-11-05/sse"
    }
  }
}
```

### Adding via Command Palette

<Steps>
  <Step title="Open the Command Palette">
    Press `Cmd+Shift+P` (macOS) or `Ctrl+Shift+P` (Windows/Linux).
  </Step>

  <Step title="Add a New MCP Server">
    Search for **MCP: Add Server** and select the command.
  </Step>

  <Step title="Choose the Transport Type">
    Select **HTTP** or **SSE** as the transport type.
  </Step>

  <Step title="Enter the Pieces MCP URL">
    Paste your MCP endpoint and name it `pieces`.
  </Step>
</Steps>

## Using Pieces MCP Server in VS Code

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in VS Code through extensions that support MCP, such as GitHub Copilot Chat.

<Steps>
  <Step title="Open the AI Chat Panel">
    Open the chat interface for your MCP-enabled extension (e.g., GitHub Copilot Chat).
  </Step>

  <Step title="Use Agent Mode">
    If your extension has chat modes, switch to *Agent* mode so it can use the `ask_pieces_ltm` tool.
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow. For example: *"What was I working on yesterday?"* or *"Show me previous implementations of this authentication method."*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

To update the URL, edit `.vscode/mcp.json` and save. VS Code picks up changes without a restart. You can also use **MCP: Edit Server** in the Command Palette to update the URL for the `pieces` server.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with VS Code:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Confirm LTM Engine Activation**: Make sure the [Long-Term Memory Engine (LTM-2.7) is enabled in PiecesOS](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine).

3. **Check Config Location**: The file must be `.vscode/mcp.json` (not `.cursor/mcp.json` or `mcp.json` at root).

4. **Verify Transport Type**: Use `type: "http"` for Streamable HTTP or `type: "sse"` for SSE. Ensure you're using the correct `servers` key (not `mcpServers`).

5. **Tools Not Visible**: Ensure your MCP-enabled extension (e.g., GitHub Copilot Chat) is installed and active. Run **MCP: List Servers** to confirm `pieces` shows as connected.

***

You're now set to enhance your VS Code workflow with powerful context retrieval through Pieces MCP. Happy coding!
