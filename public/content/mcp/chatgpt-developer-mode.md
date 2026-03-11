---
title: Pieces MCP + ChatGPT Developer Mode Integration
path: /mcp/chatgpt-developer-mode
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with ChatGPT Developer Mode lets you use Pieces Long-Term Memory in ChatGPT via the Connectors UI. Requires a remote HTTPS URL—localhost will not work.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with ChatGPT Developer Mode
metaDescription: Learn how to integrate Pieces MCP with ChatGPT Developer Mode. Requires ngrok or HTTPS proxy—ChatGPT needs a remote URL. Pro/Plus/Business/Enterprise/Education plans.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/chatgpt-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with ChatGPT Developer Mode brings your workflow context directly into ChatGPT in your browser. ChatGPT Developer Mode requires a **remote HTTPS URL**—localhost will not work. You must expose PiecesOS via [ngrok](/products/mcp/ngrok-setup) or another HTTPS proxy first.

<Callout type="alert">
  **Remote HTTPS required:** ChatGPT Developer Mode cannot use localhost. You must expose PiecesOS via ngrok or another HTTPS tunnel before adding the connector.
</Callout>

<Callout type="info">
  **Plans required:** ChatGPT Developer Mode is available on Pro, Plus, Business, Enterprise, and Education plans. Status: Beta.
</Callout>

## Prerequisites

There are **three** prerequisites for integrating Pieces with ChatGPT Developer Mode:

<Steps>
  <Step title="Supported ChatGPT Plan">
    Ensure you have a Pro, Plus, Business, Enterprise, or Education ChatGPT plan.
  </Step>

  <Step title="Install & Run PiecesOS">
    PiecesOS must be running locally. This is *required* for the MCP server to provide your workflow data.
  </Step>

  <Step title="Set Up ngrok Tunnel">
    Expose PiecesOS via an ngrok tunnel to get a public HTTPS URL. The tunnel must be active when you add the connector and when you use ChatGPT. See [ngrok Setup](/products/mcp/ngrok-setup) for detailed instructions.
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up ChatGPT Developer Mode

ChatGPT uses a Connectors UI to add MCP servers. You cannot add localhost URLs—only remote HTTPS endpoints.

### Setup Steps

<Steps>
  <Step title="Open ChatGPT">
    Open [chatgpt.com](https://chatgpt.com) in your browser.
  </Step>

  <Step title="Open Settings">
    Click your **profile icon** → **Settings**.
  </Step>

  <Step title="Go to Connectors">
    Go to **Connectors** in the sidebar.
  </Step>

  <Step title="Enable Developer Mode">
    Scroll to the bottom and click `Advanced Settings`. Toggle `Developer Mode (beta)` ON.
  </Step>

  <Step title="Create Connector">
    Return to **Connectors** and click `Create` (appears after enabling Developer Mode).
  </Step>

  <Step title="Fill in the New Connector Dialog">
    * **Connector name:** `Pieces LTM`
    * **MCP Server URL:** `https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2025-03-26/mcp`
    * **Description:** (optional) `Search and retrieve from Pieces Long-Term Memory`
  </Step>

  <Step title="Save">
    Click `Create` to save the connector.
  </Step>
</Steps>

<Callout type="info">
  The URL must point to the `/mcp` endpoint path. Subdirectory paths like `/functions/v1/mcp` do not work.
</Callout>

## Using Pieces MCP Server in ChatGPT

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in ChatGPT.

<Steps>
  <Step title="Start a New Conversation">
    Start a new conversation in ChatGPT.
  </Step>

  <Step title="Check the Tools Indicator">
    Look for the **tools indicator** in the chat.
  </Step>

  <Step title="Verify Tools">
    Ask: *"What tools do you have from Pieces?"*
  </Step>

  <Step title="Begin Prompting">
    Try: *"What did I work on yesterday?"* ChatGPT will use the `ask_pieces_ltm` tool to query your Long-Term Memory.
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

To update the ngrok URL after a tunnel restart:

1. Go to **Settings > Connectors**
2. Find "Pieces LTM" and click `Edit`
3. Update the MCP Server URL
4. Save

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with ChatGPT Developer Mode:

1. **Cannot Use localhost**: ChatGPT requires public HTTPS. Use ngrok or another HTTPS proxy.

2. **Connector Not Connecting**: Ensure the ngrok tunnel is running and the URL is accessible in a browser.

3. **Authentication Required**: Use no-auth mode; Pieces does not need OAuth.

4. **Tools Not Appearing**: Refresh the page after adding the connector.

5. **Developer Mode Not Visible**: Ensure you are on a supported plan (Pro/Plus/Business/Enterprise/Education).

6. **Write Actions Need Confirmation**: By default, writes require manual approval in ChatGPT.

***

You're now set to enhance your ChatGPT workflow with powerful context retrieval through Pieces MCP. Happy coding!
