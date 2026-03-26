---
title: Tunneling
path: /mcp/ngrok-setup
visibility: PUBLIC
status: PUBLISHED
description: Learn how to expose PiecesOS via ngrok to get a public HTTPS URL for MCP integrations that require remote access, such as ChatGPT Developer Mode and remote OpenClaw.
metaTitle: Tunneling | Pieces Docs
metaDescription: Step-by-step guide to set up ngrok with PiecesOS for remote MCP access. Required for ChatGPT Developer Mode and other integrations that need HTTPS.
---


## Tunneling with ngrok

Some MCP integrations cannot use localhost. [ChatGPT Developer Mode](/products/mcp/chatgpt-developer-mode) runs in the browser and requires a **remote HTTPS URL**. [OpenClaw](/products/mcp/openclaw) and [Claude Cowork](/products/mcp/claude-cowork) may need to reach PiecesOS from another machine. [ngrok](https://ngrok.com) creates a public HTTPS URL that forwards traffic to your local PiecesOS instance. The tunnel is active only while ngrok is running, and ngrok handles TLS certificates automatically.

<Callout type="alert">
  Exposing PiecesOS publicly via ngrok should only be used when required. For local-only integrations (Cursor, VS Code, Claude Desktop on the same machine), use localhost directly.
</Callout>

## Prerequisites

<Steps>
  <Step title="Install & Run PiecesOS">
    PiecesOS must be installed and running on the machine where you will run ngrok. Enable the Long-Term Memory Engine (LTM-2.7) through the Pieces Desktop App or the [PiecesOS Quick Menu](/products/core-dependencies/pieces-os/quick-menu).

    <pos-download-guide />
  </Step>

  <Step title="Create an ngrok Account">
    Sign up at [ngrok.com](https://ngrok.com) and get your [auth token](https://dashboard.ngrok.com/get-started/your-authtoken) from the dashboard.
  </Step>
</Steps>

## Installing ngrok

<Tabs>
  <TabItem title="macOS">
    Install with Homebrew:

    ```bash
    brew install ngrok
    ```
  </TabItem>

  <TabItem title="Windows">
    Install via the [Windows App Store](https://apps.microsoft.com/detail/9mvs1j51gmk6) or [download directly](https://ngrok.com/download).
  </TabItem>

  <TabItem title="Linux">
    On Debian/Ubuntu:

    ```bash
    curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc \
      | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null \
      && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" \
      | sudo tee /etc/apt/sources.list.d/ngrok.list \
      && sudo apt update \
      && sudo apt install ngrok
    ```
  </TabItem>
</Tabs>

Verify the installation:

```bash
ngrok help
```

## Setting Up the Tunnel

<Steps>
  <Step title="Connect your ngrok account">
    Add your auth token so ngrok can create tunnels:

    ```bash
    ngrok config add-authtoken YOUR_AUTH_TOKEN
    ```

    Replace `YOUR_AUTH_TOKEN` with the token from your [ngrok dashboard](https://dashboard.ngrok.com/get-started/your-authtoken).
  </Step>

  <Step title="Find your PiecesOS port">
    PiecesOS typically runs on port **39300**. To find yours: open the **PiecesOS Quick Menu** (system tray or menu bar) → expand **Model Context Protocol (MCP) Servers** → copy the endpoint (it includes the port). You can also find it in Pieces Desktop under **Settings** → **Model Context Protocol (MCP)**.
  </Step>

  <Step title="Start the tunnel">
    Ensure PiecesOS is running, then:

    ```bash
    ngrok http 39300
    ```

    Replace `39300` with your actual port if different. ngrok will display a forwarding URL like `https://abc123.ngrok-free.app`. Copy the **HTTPS** URL.
  </Step>
</Steps>

## MCP Endpoint URLs

Append the correct path to your ngrok URL:

| **Endpoint** | **Path** | **Use for** |
|--------------|----------|--------------|
| **Streamable HTTP (MCP)** | `/model_context_protocol/2025-03-26/mcp` | ChatGPT, Claude Cowork Connectors UI, OpenClaw (MCPorter + `mcp-remote`) |
| **SSE** | `/model_context_protocol/2024-11-05/sse` | MCP Bridge and other clients that require the legacy SSE endpoint |

Example: if ngrok shows `https://abc123.ngrok-free.app`, use `https://abc123.ngrok-free.app/model_context_protocol/2025-03-26/mcp` for ChatGPT, Claude Cowork, or OpenClaw, or `https://abc123.ngrok-free.app/model_context_protocol/2024-11-05/sse` for MCP Bridge.

## Configuring Your MCP Client

### ChatGPT Developer Mode

<Steps>
  <Step title="Open Connectors in ChatGPT">
    Open [chatgpt.com](https://chatgpt.com) → **Settings** → **Connectors**.
  </Step>
  <Step title="Create a connector">
    Click `Create` and add a new connector.
  </Step>
  <Step title="Set the MCP Server URL">
    Set **MCP Server URL** to: `https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2025-03-26/mcp`
  </Step>
  <Step title="Save and keep the tunnel running">
    Save. The tunnel must be running whenever you use ChatGPT with Pieces.
  </Step>
</Steps>

See [ChatGPT Developer Mode integration](/products/mcp/chatgpt-developer-mode) for full setup.

### Claude Cowork (Connectors UI)

<Steps>
  <Step title="Open Connectors in Claude Desktop">
    Open Claude Desktop → **Settings** → **Connectors**.
  </Step>
  <Step title="Add a custom connector">
    Click `Add custom connector`.
  </Step>
  <Step title="Paste your tunnel MCP URL">
    Enter: `https://YOUR_NGROK_URL.ngrok-free.app/model_context_protocol/2025-03-26/mcp`
  </Step>
  <Step title="Save and restart">
    Save and restart Claude Desktop.
  </Step>
</Steps>

See [Claude Cowork integration](/products/mcp/claude-cowork) for full setup.

### OpenClaw (Remote)

Install `mcp-remote` globally (`npm install -g mcp-remote@0.1.38`), then edit `~/.openclaw/workspace/config/mcporter.json`:

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

See [OpenClaw integration](/products/mcp/openclaw) for full setup.

## Tips & Troubleshooting

The tunnel is active only while `ngrok http 39300` is running. Start ngrok when you need remote access, or keep it running in a dedicated terminal for regular use.

<Callout type="info">
  Free ngrok accounts get a random subdomain each time you start a tunnel. If the URL changes, update the MCP Server URL in your client (ChatGPT: Settings → Connectors; Claude Cowork: Settings → Connectors; OpenClaw: edit `~/.openclaw/workspace/config/mcporter.json`).
</Callout>

### Troubleshooting

<Steps>
  <Step title="Tunnel not connecting">
    Ensure PiecesOS is running and listening on the port. Test locally: `curl http://localhost:39300/.well-known/version`
  </Step>
  <Step title="Wrong port">
    Use the port from the PiecesOS Quick Menu or **Settings** → **Model Context Protocol (MCP)**. It may not be 39300.
  </Step>
  <Step title="URL not accessible">
    Verify ngrok is running and the HTTPS URL loads in a browser. Free plans may show an ngrok interstitial page on first visit; that's normal.
  </Step>
  <Step title="Subdirectory paths">
    Use the exact paths: `/model_context_protocol/2025-03-26/mcp` or `/model_context_protocol/2024-11-05/sse`. Paths like `/functions/v1/mcp` do not work.
  </Step>
  <Step title="Connection refused">
    Restart PiecesOS and ngrok. Ensure no firewall is blocking the port.
  </Step>
</Steps>

### Security

ngrok exposes PiecesOS to the internet—use it only when required. Keep your ngrok auth token private. For private network access, consider [Tailscale](https://tailscale.com) or a VPN instead of a public tunnel.

***

## Next Steps

Configure your MCP client with the ngrok URL: [ChatGPT Developer Mode](/products/mcp/chatgpt-developer-mode), [Claude Cowork](/products/mcp/claude-cowork), [OpenClaw](/products/mcp/openclaw), or [MCP Bridge](/products/mcp/mcp-remote).
