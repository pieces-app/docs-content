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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/desktop/configuration/mcp/mcp_settings_overview.png" alt="" align="center" fullwidth="true" />

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

For more use cases and detailed setup instructions, refer to the [MCP documentation](/products/mcp/get-started).

***

## Next Steps

Now that you understand how to access MCP server URLs and documentation, learn how to [set up MCP with Cursor](/products/mcp/cursor) or [integrate with GitHub Copilot](/products/mcp/github-copilot) to start using Pieces Long-Term Memory in your development workflow.
