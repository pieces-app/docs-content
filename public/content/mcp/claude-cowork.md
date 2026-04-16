---
title: Pieces MCP + Claude Cowork Integration
path: /mcp/claude-cowork
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Claude Cowork lets you use Pieces Long-Term Memory in Anthropic's autonomous task automation agent. Cowork shares Claude Desktop's MCP configuration.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Claude Cowork
metaDescription: Learn how to integrate Pieces MCP with Claude Cowork. Use the same config as Claude Desktop. Pro/Max/Team/Enterprise plans. Research preview.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/claude-cowork-mcp.png" alt="Pieces MCP integration with Claude Cowork" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with Claude Cowork brings your workflow context directly into Anthropic's autonomous task automation agent. Claude Cowork is a general-purpose task automation agent that runs within Claude Desktop—it reads, writes, and organizes files, executes multi-step tasks, and works across your filesystem.

With Pieces MCP connected, Cowork can use your Long-Term Memory as context while executing tasks—like generating standups from yesterday's work or creating summary documents from your captured workflow data.

<Callout type="info">
  **Plans required:** Claude Cowork requires Pro, Max, Team, or Enterprise subscription. **Status:** Research preview (launched January 2026, Windows added February 2026).
</Callout>

## Prerequisites

<Steps>
  <Step title="Claude Desktop Installed">
    Claude Cowork runs inside Claude Desktop. Install Claude Desktop first.
  </Step>

  <Step title="Supported Plan">
    Ensure you have Pro, Max, Team, or Enterprise subscription.
  </Step>

  <Step title="Install & Run PiecesOS">
    PiecesOS must be installed and running. Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu).
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Connecting Pieces MCP to Claude Cowork

Cowork uses the **same MCP configuration as Claude Desktop**. You have two options:

### Option 1: Via Connectors UI (Pro/Max/Team/Enterprise, for remote URLs)

For remote access, you need a public HTTPS URL. Set up [ngrok](/products/mcp/ngrok-setup) or another tunnel first.

<Steps>
  <Step title="Open Claude Desktop">
    Open Claude Desktop.
  </Step>

  <Step title="Go to Connectors">
    Go to **Settings > Connectors**.
  </Step>

  <Step title="Add Custom Connector">
    Click `Add custom connector` and enter your ngrok URL:
    ```plaintext
    https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2025-03-26/mcp
    ```
  </Step>

  <Step title="Restart">
    Save and restart Claude Desktop.
  </Step>
</Steps>

### Option 2: Via JSON Config with stdio Bridge (recommended for local use)

<Callout type="info">
  **Recommended when PiecesOS and Claude Desktop are on the same machine.** Uses the localhost URL via an mcp-remote bridge.
</Callout>

Install `mcp-remote` globally with a pinned version for security:

```bash
npm install -g mcp-remote@0.1.38
```

Edit `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) or `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

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

See the [Claude Desktop guide](/products/mcp/claude-desktop) and [MCP Bridge](/products/mcp/mcp-remote) for full details.

## Using Pieces Tools in Claude Cowork

Once connected, start a Cowork session and Pieces LTM tools are available alongside file system access.

**Example tasks:**

* *"Use my Pieces Long-Term Memory to find what I worked on yesterday and write a standup to `~/Desktop/standup.md`"*
* *"Search my Pieces memory for everything I've captured about the authentication redesign and create a summary document in my project folder"*
* *"Use my Pieces audio transcriptions from today's meetings and create a meeting notes file with key decisions and action items"*

## Key Differences from Claude Chat

| Feature | Claude Chat | Claude Cowork |
|---------|-------------|---------------|
| File access | No | Yes (designated folder) |
| Task parallelism | No | Yes (sub-agents) |
| Autonomous execution | No | Yes |
| MCP tools | Yes | Yes |
| Session continuity | Per-conversation | Per-task (no cross-session memory) |

## Verification

<Steps>
  <Step title="Open a Cowork session">
    Open Claude Desktop and start a Cowork session (look for the folder/file access UI).
  </Step>
  <Step title="Confirm Pieces tools">
    Ask: *"What Pieces tools are available?"*
  </Step>
  <Step title="Try a multi-step task">
    For example: *"Search my Pieces memory for my recent work on [project name] and write a status update to my Desktop"*
  </Step>
</Steps>

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Claude Cowork:

<Steps>
  <Step title="Cowork option not visible">
    Ensure you have a Pro, Max, Team, or Enterprise plan.
  </Step>
  <Step title="Pieces tools not appearing">
    Restart Claude Desktop after config changes.
  </Step>
  <Step title="MCP tools unavailable">
    Confirm the Pieces server is configured in Claude Desktop—Cowork shares Desktop's config.
  </Step>
  <Step title="Windows">
    Windows support was added February 10, 2026—update Claude Desktop.
  </Step>
</Steps>

***

You're now set to enhance your Claude Cowork workflow with powerful context retrieval through Pieces MCP. Happy coding!
