---
title: Pieces MCP + OpenAI Codex CLI Integration
path: /mcp/openai-codex-cli
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with OpenAI Codex CLI lets you use Pieces Long-Term Memory directly from the Codex command-line agent.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with OpenAI Codex CLI
metaDescription: Learn how to integrate Pieces MCP with OpenAI Codex CLI. Use TOML config format for MCP server setup. Requires Codex 0.2.0+.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/codex-mcp.png" alt="Pieces MCP integration with OpenAI Codex CLI" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp) with OpenAI Codex CLI brings your workflow context directly into the Codex command-line agent. Codex uses **TOML** (not JSON) for its configuration.

<Callout type="info">
  **Minimum version:** Codex CLI 0.2.0 or later is required for MCP support.
</Callout>

## Prerequisites

There are **two** prerequisites for integrating Pieces with Codex CLI as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up OpenAI Codex CLI

Codex stores its MCP configuration in `~/.codex/config.toml`. The file format is **TOML**, not JSON.

### Config File Location

| Scope | Path |
|-------|------|
| **User (global)** | `~/.codex/config.toml` |
| **Project** | `.codex/config.toml` at project root (trusted projects only) |

### Local Setup (Streamable HTTP — recommended)

Edit `~/.codex/config.toml`:

```toml
[mcp_servers.pieces]
url = "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
startup_timeout_sec = 10
tool_timeout_sec = 60
```

### Optional: Filter Specific Tools

To only expose specific Pieces tools:

```toml
[mcp_servers.pieces]
url = "http://localhost:39300/model_context_protocol/2025-03-26/mcp"
enabled_tools = ["ask_pieces_ltm", "workstream_summaries_full_text_search"]
```

## Using Pieces MCP Server in Codex CLI

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Codex.

<Steps>
  <Step title="Start a Codex Session">
    Run `codex` in your terminal.
  </Step>

  <Step title="Verify Tools">
    Codex announces available MCP tools on startup. Ask: *"What Pieces tools are available?"*
  </Step>

  <Step title="Begin Prompting">
    Ask context-rich questions about your workflow.
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit `~/.codex/config.toml`, update the `url`, and run a new Codex session.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Codex CLI:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system. Verify the URL responds.

2. **Use TOML, Not JSON**: Codex uses TOML format. Creating a `.json` file will not work.

3. **Update Codex**: MCP support requires Codex CLI 0.2.0 or later.

4. **Config File Not Found**: Create `~/.codex/config.toml` manually.

5. **Timeout Errors**: Increase `startup_timeout_sec` or `tool_timeout_sec` if you encounter timeouts.

***

You're now set to enhance your Codex CLI workflow with powerful context retrieval through Pieces MCP. Happy coding!
