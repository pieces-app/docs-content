---
title: Pieces MCP + OpenClaw Integration
path: /mcp/openclaw
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with OpenClaw lets you use Pieces Long-Term Memory in the open-source self-hosted AI agent that runs 24/7 and connects to messaging platforms.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with OpenClaw
metaDescription: Learn how to integrate Pieces MCP with OpenClaw. OpenClaw executes MCP tools via MCPorter. Automate standups, meeting prep, and more.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/openclaw-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with OpenClaw brings your workflow context directly into this open-source continuous AI agent runtime. OpenClaw (formerly ClawdBot, formerly Moltbot) runs as a persistent Node.js service—unlike chatbots that respond to one-off prompts, it runs 24/7, executing tasks proactively via cron jobs and event listeners.

With Pieces MCP connected, OpenClaw gains access to your Long-Term Memory. It can autonomously query your past work, generate standups, monitor recent activity, and surface relevant context without you asking.

## Prerequisites

<Steps>
  <Step title="Node.js 18+">
    Install Node.js 18 or later.
  </Step>

  <Step title="OpenClaw Installed">
    Clone and configure OpenClaw following the [OpenClaw setup guide](https://github.com/clawdbot).
  </Step>

  <Step title="Install & Run PiecesOS">
    PiecesOS must be running locally (port 39300-39333). Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu).
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up OpenClaw

OpenClaw executes MCP tools via **MCPorter**, its built-in MCP management layer. Edit `~/.openclaw/workspace/config/mcporter.json`:

Install `mcp-remote` globally with a pinned version for security:

```bash
npm install -g mcp-remote@0.1.38
```

See [MCP Bridge](/products/mcp/mcp-remote) for why we recommend a locally installed binary over `npx`.

### Local Setup (SSE with mcp-remote — recommended)

When OpenClaw and PiecesOS run on the same machine, use the localhost URL with the mcp-remote bridge:

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

### Remote Setup (ngrok)

When OpenClaw needs to reach PiecesOS on a different machine:

```json
{
  "mcpServers": {
    "pieces": {
      "command": "mcp-remote",
      "args": [
        "https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2024-11-05/sse"
      ]
    }
  }
}
```

See [Tunneling](/products/mcp/ngrok-setup) for tunnel setup.

## Example Use Cases

Once Pieces MCP is connected to OpenClaw, you can automate workflows like:

**Autonomous daily standup:** Schedule OpenClaw to run every morning, query yesterday's workstream summaries, and post a formatted standup to your Slack or Teams channel.

**Meeting prep:** Before a calendar event, OpenClaw searches audio transcriptions and workstream summaries for context related to the meeting topic and drafts a brief for you.

**Automated debugging log:** When OpenClaw detects a production alert, it queries recent workstream events for error-related content and creates a pieces_memory entry with the incident context.

## Verification

1. Start OpenClaw.
2. Ask via your connected messaging platform: *"What Pieces tools do you have?"*
3. Pieces LTM tools should be listed.
4. Try: *"What did I work on yesterday?"*—OpenClaw will call `ask_pieces_ltm`.

## Security Note

OpenClaw can run with `permissionMode: 'bypassPermissions'` to execute tools autonomously. When combined with Pieces MCP write tools (like `create_pieces_memory`), this is powerful but should be used carefully. Consider:

* Running OpenClaw in Docker with limited filesystem access
* Disabling write tools in MCPorter if running fully autonomously
* Monitoring execution logs

## Updating

Edit `~/.openclaw/workspace/config/mcporter.json`, update the URL, and restart OpenClaw.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with OpenClaw:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **MCPorter Config Not Found**: Create `~/.openclaw/workspace/config/` directory manually.

3. **Bridge Process Not Starting**: Run `npm install -g mcp-remote@0.1.38` and ensure the global npm bin directory is in your PATH.

4. **Tools Not Available**: Restart OpenClaw after editing MCPorter config.

5. **ngrok URL Expired**: Restart the ngrok tunnel and update the URL in MCPorter config. See [ngrok Setup](/products/mcp/ngrok-setup) for details.

***

You're now set to enhance your OpenClaw workflow with powerful context retrieval through Pieces MCP. Happy coding!
