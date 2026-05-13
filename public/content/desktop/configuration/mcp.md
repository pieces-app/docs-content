---
title: Model Context Protocol (MCP)
path: /desktop/configuration/mcp
visibility: PUBLIC
status: PUBLISHED
description: Access MCP server URLs and documentation to integrate Pieces Long-Term Memory with Cursor, GitHub Copilot, and other tools.
metaTitle: Model Context Protocol (MCP) Settings in Pieces Desktop
metaDescription: Access MCP server URLs and documentation to integrate Pieces Long-Term Memory with Cursor, GitHub Copilot, and other tools.
---

## Model Context Protocol (MCP) Settings

Access server URLs and documentation for integrating Pieces Long-Term Memory with Cursor, GitHub Copilot, and other tools that support the Model Context Protocol. The MCP server enables connectivity between Large Language Models (LLMs) and your personal context stored by the Long-Term Memory Engine (LTM-2.7).

To access MCP settings, click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/MCP/mcp_settings_overview.png" alt="Model Context Protocol settings showing server URLs and documentation" align="center" fullwidth="true" />

> Model Context Protocol (MCP) settings showing server URLs and View Documentation option

## Available Servers

Copy the server URLs to configure MCP integrations in compatible IDEs and code editors. Multiple server URLs are available, including the latest schema version and previous versions for compatibility.

### Understanding Server URLs

The MCP settings display server URLs that your development tools or AI applications, such as [Cursor](/products/mcp/cursor) or [GitHub Copilot](/products/mcp/github-copilot), will use to communicate directly with your local PiecesOS MCP server.

<Callout type="info">
  Copy the server URL below and paste it into your MCP client configuration. The latest schema version may not be compatible with all MCP clients yet. If you experience connection issues, try using an earlier version or restarting your MCP client. For the best results, try using with Cursor or Claude.
</Callout>

### Copying Server URLs

<Steps>
  <Step title="Open MCP Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.
  </Step>

  <Step title="Locate Available Servers Section">
    In the *Available Servers* section, you'll see server URLs displayed, each with a Copy Icon to the right.
  </Step>

  <Step title="Copy Latest Schema URL">
    The latest schema URL is marked with a blue "LATEST SCHEMA" badge. Click the `Copy Icon` next to the URL to copy it to your clipboard. The URL format is `http://localhost:39300/model_context_protocol/2025-03-26/mcp` with the release date displayed below it.
  </Step>

  <Step title="Copy Previous Version URL (Optional)">
    If you need compatibility with older MCP clients, you can copy a previous version URL (e.g., `http://localhost:39300/model_context_protocol/2024-11-05/sse`). Click the `Copy Icon` next to the URL you need.
  </Step>

  <Step title="Use in Integration">
    Paste the copied URL into your IDE or tool's MCP configuration. Use the latest schema URL for the most up-to-date features, or use an earlier version if you encounter compatibility issues.
  </Step>
</Steps>

<Callout type="info">
  The release date displayed under each server URL indicates when that schema version was released. The latest schema version provides the most current features, but older versions may be more compatible with certain MCP clients.
</Callout>

## View Documentation

Access detailed guides that explain how to leverage MCP integrations with popular development environments, such as Cursor and GitHub Copilot.

### Opening MCP Documentation

<Steps>
  <Step title="Open MCP Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.
  </Step>

  <Step title="Locate View Documentation Section">
    Scroll to the *View Documentation* section, which displays: "Learn how to use Long-Term Memories with Cursor, GitHub Copilot and other tools using our MCP server."
  </Step>

  <Step title="Click Documentation Icon">
    Click the `Documentation Icon` (book icon) to open the MCP documentation, which covers setup instructions, example scenarios, and troubleshooting tips for efficient MCP usage.
  </Step>
</Steps>

The documentation provides comprehensive guides on:

* **Setting Up Integrations**: Step-by-step instructions for configuring MCP in Cursor, GitHub Copilot, and other tools
* **Use Cases**: Examples of how MCP enhances your coding and debugging experiences
* **Troubleshooting**: Solutions for common integration issues and configuration problems

### Example Use Cases

MCP enhances your coding and debugging experiences in several ways:

* **Context-Rich Debugging**: Instantly retrieve logs, historical debugging notes, or team discussions directly from PiecesOS when troubleshooting within Cursor
* **Contextual Queries**: Access historical code implementations, error resolutions, or previously encountered bugs within GitHub Copilot for quicker coding solutions

For more use cases and detailed setup instructions, refer to the [MCP documentation](/products/mcp).

## MCP Connections

Connect Pieces to supported MCP clients with one click. Pieces writes to each client's global or user-level MCP config and, when supported, also creates the matching global rule or skill file automatically.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/MCP/mcp_connections_section.png" alt="MCP Connections section showing supported clients with Connect buttons" align="center" fullwidth="true" />

> MCP Connections section showing supported clients with one-click Connect buttons

<Callout type="info">
  Some MCP clients may need to be restarted or reopened before configuration changes appear.
</Callout>

The MCP Connections section shows your connection status (e.g., "Connected 4 of 6") and a `Refresh Connections` button to update the status.

### Supported Clients

| Client | Description |
| --- | --- |
| **Claude Desktop** | Connect Pieces to Claude Desktop for memory-backed conversations |
| **Cursor** | Connect Pieces to Cursor so your IDE has access to long-term memory |
| **GitHub Copilot** | Connect Pieces to GitHub Copilot for context-aware code suggestions |
| **Codex** | Connect Pieces to Codex so both the CLI and IDE extension can connect to your memory via MCP |
| **Google Gemini CLI** | Connect Pieces to Google Gemini CLI so terminal-based workflows can use MCP-backed context |
| **Antigravity** | Connect Pieces to Antigravity so its agent panel can access your long-term memory over MCP |
| **Claude Code** | Connect Pieces to Claude Code so terminal-based workflows can use long-term memory context |
| **OpenClaw** | OpenClaw setup is documented separately for now. Click `View Docs` to open the setup guide |

### Connecting a Client

<Steps>
  <Step title="Open MCP Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.
  </Step>
  <Step title="Scroll to MCP Connections">
    Find the *MCP Connections* section below the Available Servers and View Documentation sections.
  </Step>
  <Step title="Click Connect">
    Click the `Connect` button next to the client you want to configure. Pieces automatically writes the MCP configuration to that client's config file.
  </Step>
  <Step title="Restart the Client">
    Restart or reopen the MCP client for the configuration changes to take effect.
  </Step>
</Steps>

### Managing Connected Clients

Once connected, a green checkmark appears next to the client name. To disconnect or reconfigure:

<Steps>
  <Step title="Click the Three-Dot Menu">
    Click the `⋮` menu next to a connected client.
  </Step>
  <Step title="Choose an Action">
    Select **Disconnect** to remove the configuration, or **Reconfigure** to update settings.
  </Step>
</Steps>

<Callout type="tip">
  OpenClaw requires manual configuration. If your OpenClaw instance is remote (e.g., a homelab server), you'll need to set up tunneling. Click `View Docs` next to OpenClaw to see the setup guide.
</Callout>

***

## Next Steps

Now that you understand how to access MCP server URLs and documentation, learn how to [set up MCP with Cursor](/products/mcp/cursor) or [integrate with GitHub Copilot](/products/mcp/github-copilot) to start using Pieces Long-Term Memory in your development workflow.
