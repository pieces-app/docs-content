---
title: Pieces MCP + Antigravity Integration
path: /mcp/antigravity
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Antigravity lets you use Pieces Long-Term Memory directly in the Antigravity agent panel.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Antigravity
metaDescription: Learn how to integrate Pieces MCP with Antigravity. Connect your long-term memory to the Antigravity agent panel for context-aware assistance.
---

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Antigravity brings your workflow context directly into the Antigravity agent panel. With this integration, the Antigravity agent can access your long-term memory over MCP for context-aware assistance.

## Prerequisites

There are **two** prerequisites for integrating Pieces with Antigravity as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

<Steps>
  <Step title="Install & Run PiecesOS">
    Make sure that PiecesOS is installed and running. This is *required* for the MCP server to communicate with your workflow data.

    If you do not have PiecesOS, you can download it alongside the [Pieces Desktop App](/products/desktop/download) or [install it standalone](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation).
  </Step>

  <Step title="Enable Long-Term Memory">
    Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) in your toolbar.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up Antigravity

### One-Click Setup via Pieces Desktop (Recommended)

The fastest way to connect Pieces MCP to Antigravity is through the MCP Connections feature in Pieces Desktop.

<Steps>
  <Step title="Open MCP Settings">
    In Pieces Desktop, click your `User Profile` in the top left, then hover over `Settings` and select `MCP`.
  </Step>

  <Step title="Find MCP Connections">
    Scroll down to the *MCP Connections* section. You'll see a list of supported clients with `Connect` buttons.
  </Step>

  <Step title="Click Connect">
    Click the `Connect` button next to **Antigravity**. Pieces automatically writes the MCP configuration.
  </Step>

  <Step title="Handle Missing Dependencies (if prompted)">
    If Pieces detects missing dependencies, a dialog appears with installation instructions. Follow the steps shown, then click `Retry`.
  </Step>

  <Step title="Restart Antigravity">
    Restart or reopen Antigravity for the configuration changes to take effect. Once connected, a green checkmark appears next to Antigravity in the MCP Connections list.
  </Step>
</Steps>

<Callout type="info">
  To disconnect later, click the `⋮` menu next to the connected client and select **Disconnect**, or click the red `✕` next to the connection entry.
</Callout>

### Manual Configuration

If you prefer manual setup, add the Pieces MCP server URL to your Antigravity configuration:

```text
http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

<Callout type="info">
  The port number (`39300`) may vary depending on your PiecesOS installation. Check the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu) for the active MCP endpoint.
</Callout>

## Using Pieces MCP Server in Antigravity

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Antigravity's agent panel.

<Steps>
  <Step title="Open the Agent Panel">
    Launch Antigravity and open the agent panel.
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow, such as:
    * *"What was I working on yesterday?"*
    * *"Show me the code changes I made related to authentication."*
    * *"What did my team discuss about the API redesign?"*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Antigravity:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Confirm LTM Engine Activation**: Make sure the [Long-Term Memory Engine (LTM-2.7) is enabled in PiecesOS](/products/core-dependencies/pieces-os/quick-menu#ltm-2-engine).

3. **Check Connection Status**: In Pieces Desktop, go to Settings → MCP → MCP Connections and verify that Antigravity shows a green checkmark.

4. **Restart After Configuration**: Antigravity may need to be restarted after configuration changes.

5. **Review MCP Endpoint**: Double-check the MCP endpoint URL and port number in your configuration.

***

You're now set to enhance your Antigravity workflow with powerful context retrieval through Pieces MCP.
