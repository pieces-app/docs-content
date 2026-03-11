---
title: MCP Bridge
path: /mcp/mcp-remote
visibility: PUBLIC
status: PUBLISHED
description: Learn how to use the mcp-remote stdio bridge to connect stdio-only MCP clients to PiecesOS, enabling Pieces Long-Term Memory in Raycast, Zed, Claude Cowork, and more.
metaTitle: MCP Bridge | Pieces Docs
metaDescription: Use mcp-remote to connect stdio-only MCP clients to PiecesOS. Step-by-step guide for Raycast, Zed, Claude Cowork, OpenClaw, and remote setups.
---

## MCP Bridge

Many MCP clients—including Raycast, Zed, and Claude Cowork—only support **stdio** (standard input/output) connections. PiecesOS exposes its MCP server over **HTTP** and **SSE**. The [mcp-remote](https://www.npmjs.com/package/mcp-remote) bridge translates between these protocols so stdio-only clients can connect to PiecesOS and use [Pieces Long-Term Memory](/products/core-dependencies/pieces-os#ltm-27).

<Callout type="tip">
  The easiest way to bridge MCP is with the Pieces CLI—run `pieces mcp setup` and select your platform. Use manual setup below only for clients not supported by the CLI or when you need custom config (e.g., remote URLs).
</Callout>

## Easiest Option: Pieces CLI

The [Pieces CLI](/products/cli/get-started) automatically configures MCP for supported platforms—no manual config editing required.

<Steps>
  <Step title="Run the setup command">
    In your terminal, run `pieces mcp setup`.
  </Step>
  <Step title="Select your platform">
    Use the arrow keys to select your MCP client (VS Code, Cursor, Claude Desktop, Windsurf, Claude Code, Raycast, or Warp) and press Enter.
  </Step>
  <Step title="Confirm">
    The CLI updates the platform's config file and confirms when Pieces MCP is enabled.
  </Step>
</Steps>

<Callout type="info">
  Ensure PiecesOS is running and LTM is enabled. Run `pieces mcp status` to verify your setup.
</Callout>

## Manual Setup

Use manual setup when your client isn't supported by the CLI (e.g Zed and OpenClaw) or when you need to point at a remote PiecesOS URL (see [Tunneling](/products/mcp/ngrok-setup)).

### Prerequisites

<Steps>
  <Step title="Install & Run PiecesOS">
    PiecesOS must be installed and running. Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu).

    <pos-download-guide />
  </Step>

  <Step title="Install Node.js">
    `mcp-remote` requires Node.js 18+. Ensure Node.js and `npm` are in your PATH.
  </Step>

  <Step title="Install mcp-remote (version-pinned)">
    Install `mcp-remote` globally with a pinned version so your MCP client runs a known, verified binary instead of fetching from the registry at runtime:

    ```bash
    npm install -g mcp-remote@0.1.38
    ```

    <Callout type="alert">
      Using `npx` to run `mcp-remote` downloads the package from npm each time. For better security, use a locally installed, version-pinned binary as shown above.
    </Callout>
  </Step>
</Steps>

### Pieces MCP Endpoints

PiecesOS exposes two endpoints. For `mcp-remote`, use the **SSE** endpoint—it works reliably across all stdio clients:

| **Endpoint** | **URL** | **Use for** |
|--------------|---------|--------------|
| **SSE** | `http://localhost:39300/model_context_protocol/2024-11-05/sse` | mcp-remote, stdio clients |
| **Streamable HTTP** | `http://localhost:39300/model_context_protocol/2025-03-26/mcp` | Clients that support HTTP natively |

<Callout type="alert">
  The port may vary. Find yours in the PiecesOS Quick Menu under **Model Context Protocol (MCP) Servers**, or in Pieces Desktop under **Settings** → **Model Context Protocol (MCP)**.
</Callout>

### Configuring Your Client

<Tabs>
  <TabItem title="Raycast">
    Edit `mcp-config.json` (open via **Manage MCP Servers** → **Show Config File in Finder**):

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

    See [Raycast integration](/products/mcp/raycast) for full setup.
  </TabItem>

  <TabItem title="Zed">
    Zed uses `context_servers` (not `mcpServers`). Edit your Zed `settings.json`:

    ```json
    {
      "context_servers": {
        "pieces": {
          "command": {
            "path": "mcp-remote",
            "args": [
              "http://localhost:39300/model_context_protocol/2024-11-05/sse"
            ],
            "env": {}
          },
          "settings": {}
        }
      }
    }
    ```

    See [Zed integration](/products/mcp/zed) for full setup.
  </TabItem>

  <TabItem title="Claude Cowork">
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

    See [Claude Cowork integration](/products/mcp/claude-cowork) for full setup.
  </TabItem>

  <TabItem title="OpenClaw">
    Edit `~/.openclaw/workspace/config/mcporter.json`:

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

    See [OpenClaw integration](/products/mcp/openclaw) for full setup.
  </TabItem>
</Tabs>

For remote setups, use the ngrok URL instead of localhost. See [Tunneling](/products/mcp/ngrok-setup).

### Useful Flags

| **Flag** | **Purpose** |
|----------|-------------|
| `--allow-http` | Allow HTTP URLs; use only in trusted private networks |
| `--debug` | Write verbose logs to `~/.mcp-auth/{hash}_debug.log` |
| `--silent` | Suppress default logs |

## Tips & Troubleshooting

Ensure PiecesOS is running. Test the endpoint: `curl http://localhost:39300/.well-known/version`. Restart your MCP client after changing config, then ask: *"What tools do you have from Pieces?"* or *"What did I work on yesterday?"*

### Troubleshooting

1. **mcp-remote: command not found** — Run `npm install -g mcp-remote@0.1.38` and ensure the global npm bin directory is in your PATH.

2. **Bridge not connecting** — Verify PiecesOS is running and the port is correct. Test with `curl http://localhost:39300/.well-known/version`.

3. **Wrong config key** — Zed uses `context_servers`; Raycast, Claude Cowork, and OpenClaw use `mcpServers`.

4. **Port mismatch** — Check the PiecesOS Quick Menu or Settings → Model Context Protocol (MCP) for the current endpoint.

5. **Stale credentials** — If you have persistent issues, try `rm -rf ~/.mcp-auth` and restart the client.

***

## Next Steps

* [Raycast](/products/mcp/raycast) — macOS launcher with Pieces LTM
* [Zed](/products/mcp/zed) — Zed editor with Pieces LTM
* [Claude Cowork](/products/mcp/claude-cowork) — Claude Cowork with Pieces LTM
* [OpenClaw](/products/mcp/openclaw) — OpenClaw with Pieces LTM
* [Tunneling](/products/mcp/ngrok-setup) — Expose PiecesOS for remote MCP access
