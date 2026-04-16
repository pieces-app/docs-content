---
title: Pieces MCP + OpenClaw Integration
path: /mcp/openclaw
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with OpenClaw lets you use Pieces Long-Term Memory in the open-source self-hosted AI agent that runs 24/7 and connects to messaging platforms.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with OpenClaw
metaDescription: Learn how to integrate Pieces MCP with OpenClaw. OpenClaw executes MCP tools via MCPorter. Automate standups, meeting prep, and more.
---

<Embed
  src="https://youtu.be/Bh_y65oGzMg"
  title="Pieces MCP integration with OpenClaw walkthrough"
/>

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with OpenClaw brings your workflow context directly into this open-source continuous AI agent runtime. OpenClaw (formerly ClawdBot, formerly Moltbot) runs as a persistent Node.js service—unlike chatbots that respond to one-off prompts, it runs 24/7, executing tasks proactively via cron jobs and event listeners.

With Pieces MCP connected, OpenClaw gains access to your Long-Term Memory. It can autonomously query your past work, generate standups, monitor recent activity, and surface relevant context without you asking.

## Prerequisites

<Steps>
  <Step title="Node.js 18+">
    Install Node.js 18 or later.
  </Step>

  <Step title="OpenClaw Installed">
    Clone and configure OpenClaw following the [setup instructions in the OpenClaw getting started](https://docs.openclaw.ai/start/getting-started).
  </Step>

  <Step title="Official Pieces skill on ClawHub">
    Install the [Pieces Long-Term Memory (MCP) skill](https://clawhub.ai/jackrosspieces/pieces-mcp) on ClawHub. It is the full agent-facing guide for OpenClaw: MCP-only URLs, tunnels when PiecesOS runs on another machine, `mcporter.json`, `mcp-remote`, gateway restart, and troubleshooting.
  </Step>

  <Step title="Install & Run PiecesOS">
    PiecesOS must be running locally (port 39300-39333). Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu).
  </Step>
</Steps>

### Installing PiecesOS & Configuring Permissions

Follow the instructions below for a detailed guide on setting up and configuring PiecesOS to correctly pass captured workflow context to the Pieces MCP server.

<pos-download-guide />

## Setting Up OpenClaw

OpenClaw executes MCP tools via **MCPorter**, its built-in MCP management layer. Edit `~/.openclaw/workspace/config/mcporter.json`.

The [official Pieces MCP skill for OpenClaw](https://clawhub.ai/jackrosspieces/pieces-mcp) documents **MCP-only** integration: point `mcp-remote` at the **`/mcp`** endpoint (`/model_context_protocol/2025-03-26/mcp`), not the legacy **`/sse`** path. That matches how OpenClaw and MCPorter expect to bridge Pieces.

Install `mcp-remote` globally with a pinned version for security:

```bash
npm install -g mcp-remote@0.1.38
```

See [MCP Bridge](/products/mcp/mcp-remote) for why we recommend a locally installed binary over `npx`.

### Local setup (MCP with mcp-remote — recommended)

When OpenClaw and PiecesOS run on the same machine, use the localhost MCP URL with the mcp-remote bridge:

```json
{
  "mcpServers": {
    "pieces": {
      "command": "mcp-remote",
      "args": [
        "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
      ]
    }
  }
}
```

### Remote setup (ngrok or other HTTPS tunnel)

When OpenClaw runs on a different machine than PiecesOS, expose PiecesOS (port 39300) with a tunnel and use the **same MCP path** on your tunnel base URL:

```json
{
  "mcpServers": {
    "pieces": {
      "command": "mcp-remote",
      "args": [
        "https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2025-03-26/mcp"
      ]
    }
  }
}
```

See [Tunneling](/products/mcp/ngrok-setup) for tunnel setup. For step-by-step tunnel checks, `curl` validation, and gateway restarts, follow the [ClawHub skill](https://clawhub.ai/jackrosspieces/pieces-mcp).

## Example Use Cases

Once Pieces MCP is connected to OpenClaw, you can automate workflows like:

**Autonomous daily standup:** Schedule OpenClaw to run every morning, query yesterday's workstream summaries, and post a formatted standup to your Slack or Teams channel.

**Meeting prep:** Before a calendar event, OpenClaw searches audio transcriptions and workstream summaries for context related to the meeting topic and drafts a brief for you.

**Automated debugging log:** When OpenClaw detects a production alert, it queries recent workstream events for error-related content and creates a pieces_memory entry with the incident context.

## Verification

<Steps>
  <Step title="Start OpenClaw">
    Launch or connect to your OpenClaw instance as you normally do.
  </Step>
  <Step title="Confirm Pieces tools are exposed">
    Ask via your connected messaging platform: *"What Pieces tools do you have?"* Pieces LTM tools should appear in the list.
  </Step>
  <Step title="Exercise Long-Term Memory">
    Try: *"What did I work on yesterday?"*—OpenClaw should call `ask_pieces_ltm`.
  </Step>
</Steps>

## Security Note

OpenClaw can run with `permissionMode: 'bypassPermissions'` to execute tools autonomously. When combined with Pieces MCP write tools (like `create_pieces_memory`), this is powerful but should be used carefully. Consider:

* Running OpenClaw in Docker with limited filesystem access
* Disabling write tools in MCPorter if running fully autonomously
* Monitoring execution logs

## Updating

Edit `~/.openclaw/workspace/config/mcporter.json`, update the URL, then restart the OpenClaw gateway (for example `openclaw gateway restart` from `~/.openclaw/workspace`, as in the [official skill](https://clawhub.ai/jackrosspieces/pieces-mcp)).

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with OpenClaw:

<Steps>
  <Step title="Verify PiecesOS is running">
    Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.
  </Step>
  <Step title="MCPorter config path exists">
    If the config is missing, create `~/.openclaw/workspace/config/` manually.
  </Step>
  <Step title="Bridge process (`mcp-remote`)">
    Run `npm install -g mcp-remote@0.1.38` and ensure the global npm bin directory is in your `PATH`.
  </Step>
  <Step title="Tools still not listed">
    After editing MCPorter config, restart the gateway (`openclaw gateway restart` per the [ClawHub skill](https://clawhub.ai/jackrosspieces/pieces-mcp)) so OpenClaw picks up the Pieces MCP server.
  </Step>
  <Step title="Remote / tunnel URL">
    If you use ngrok or another tunnel, restart the tunnel when the URL changes and update the URL in MCPorter config. See [ngrok Setup](/products/mcp/ngrok-setup) for details.
  </Step>
</Steps>

***

You're now set to enhance your OpenClaw workflow with powerful context retrieval through Pieces MCP. Happy coding!
