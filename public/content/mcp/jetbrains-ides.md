---
title: Pieces MCP + JetBrains IDEs Integration
path: /mcp/jetbrains-ides
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with JetBrains IDEs (IntelliJ IDEA, PyCharm, WebStorm, GoLand, etc.) lets you use Pieces Long-Term Memory directly in your IDE via the AI Assistant.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with JetBrains IDEs
metaDescription: Learn how to integrate Pieces MCP with JetBrains IDEs. Requires JetBrains 2025.2+ with AI Assistant. Access Long-Term Memory for enhanced productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/jetbrains-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with JetBrains IDEs brings your workflow context directly into IntelliJ IDEA, PyCharm, WebStorm, GoLand, and other JetBrains editors. The AI Assistant can access your past work, similar code, and historical context.

<Callout type="info">
  **Minimum version:** JetBrains 2025.2 or later is required for MCP support. SSE has limited/deprecated support—use Streamable HTTP for best results.
</Callout>

## Prerequisites

There are **two** prerequisites for integrating Pieces with JetBrains as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up JetBrains IDEs

JetBrains provides an MCP setup UI in Settings. You do not need to edit config files manually.

### Setup via Settings UI

<Steps>
  <Step title="Open Settings">
    Go to **Settings** (`Cmd+,` on macOS, `Ctrl+Alt+S` on Windows/Linux).
  </Step>

  <Step title="Navigate to MCP">
    Go to **Tools > AI Assistant > Model Context Protocol (MCP)**.
  </Step>

  <Step title="Add a New Server">
    Click `+` (Add) to create a new server. In the **New MCP Server** dialog, enter the Pieces MCP URL:
    ```plaintext
    http://localhost:39300/model_context_protocol/2025-03-26/mcp
    ```
  </Step>

  <Step title="Set Transport Type">
    Select **Streamable HTTP** as the transport type. Optionally set a working directory.
  </Step>

  <Step title="Apply">
    Click `OK` to apply your changes.
  </Step>
</Steps>

### Brave Mode (Auto-Execute Tools)

By default, JetBrains prompts for confirmation before executing tools. To enable auto-execution:

Go to **Settings > Tools > AI Assistant > MCP > Brave Mode = enabled**

<Callout type="warning">
  Use Brave Mode with caution in production environments.
</Callout>

## Using Pieces MCP Server in JetBrains

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in the AI Assistant panel.

<Steps>
  <Step title="Open the AI Assistant Panel">
    Open the **AI Assistant** panel in your JetBrains IDE.
  </Step>

  <Step title="Verify Tools">
    Check that Pieces tools appear in the available tools list.
  </Step>

  <Step title="Begin Prompting">
    Ask the AI Assistant to query your Pieces Long-Term Memory. For example: *"What was I working on yesterday?"*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Go to **Settings > Tools > AI Assistant > MCP**, select the `pieces` server, click `Edit`, update the URL, and apply.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with JetBrains:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Update JetBrains**: MCP support requires JetBrains 2025.2 or later. If the MCP option is not visible, update your IDE.

3. **Use Streamable HTTP**: JetBrains has limited/deprecated SSE support. Use the Streamable HTTP endpoint (`/model_context_protocol/2025-03-26/mcp`).

4. **AI Not Using Tools Automatically**: Enable **Brave Mode** in MCP settings if the AI is not executing tools automatically.

***

You're now set to enhance your JetBrains workflow with powerful context retrieval through Pieces MCP. Happy coding!
