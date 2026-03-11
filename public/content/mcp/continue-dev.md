---
title: Pieces MCP + Continue.dev Integration
path: /mcp/continue-dev
visibility: PUBLIC
status: PUBLISHED
description: The Pieces MCP integration with Continue.dev lets you use Pieces Long-Term Memory directly in VS Code or JetBrains IDEs via the open-source Continue.dev extension, in agent mode.
metaTitle: Integrate Pieces Model Context Protocol (MCP) with Continue.dev
metaDescription: Learn how to integrate Pieces MCP with Continue.dev. Access Long-Term Memory in agent mode for enhanced, context-aware productivity.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/mcp_cover_images/continuedev-mcp.png" alt="" align="center" fullwidth="true" />

***

## Get Started

Integrating the [Pieces MCP](/products/mcp/get-started) with Continue.dev brings your workflow context directly into your editor. Continue.dev is an open-source coding assistant available as a VS Code or JetBrains extension.

<Callout type="info">
  **Agent mode required:** MCP servers in Continue.dev only work in **agent mode**. They are not available in regular chat or plan modes.
</Callout>

## Prerequisites

There are **two** prerequisites for integrating Pieces with Continue.dev as an MCP—an active instance of **PiecesOS** and the fully-enabled **Long-Term Memory** engine.

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

## Setting Up Continue.dev

Continue.dev uses **YAML** configuration with an `mcpServers` array. The recommended location is `.continue/config.yaml` at your project root (you can commit it to version control for team sharing).

### Config File Location

| Scope | Path |
|-------|------|
| **Workspace (recommended)** | `.continue/config.yaml` at project root |
| **Alternative JSON** | `.continue/mcpServers/mcp.json` |

### Local Setup (Streamable HTTP — recommended)

Create or edit `.continue/config.yaml`:

```yaml
mcpServers:
  - name: Pieces LTM
    type: streamable-http
    url: http://localhost:39300/model_context_protocol/2025-03-26/mcp
```

### Local Setup (SSE)

```yaml
mcpServers:
  - name: Pieces LTM
    type: sse
    url: http://localhost:39300/model_context_protocol/2024-11-05/sse
```

<Callout type="alert">
  Use `streamable-http` (with hyphen), not `streamableHttp` or `http`. The type value is case-sensitive.
</Callout>

## Using Pieces MCP Server in Continue.dev

Once integrated, you can utilize [Pieces LTM](/products/core-dependencies/pieces-os#ltm-27) directly in Continue.dev.

<Steps>
  <Step title="Switch to Agent Mode">
    Switch Continue.dev to **agent mode** in the UI. MCP servers are only available in agent mode.
  </Step>

  <Step title="Verify Tools">
    Check the available tools—Pieces LTM tools should appear.
  </Step>

  <Step title="Begin Prompting">
    Ask the agent to search your Long-Term Memory. For example: *"What was I working on yesterday?"*
  </Step>
</Steps>

<Card title="Hey!" image="/assets/icons/platform_logos/pieces_logo.png">
  Check out this [MCP-specific prompting guide](/products/mcp/prompting) if you want to effectively utilize the Long-Term Memory Engine (LTM-2.7) with your new Pieces MCP server.
</Card>

## Updating

Edit your `config.yaml` (or JSON file), update the `url`, and switch to agent mode. Continue picks up the change on the next agent session.

## Troubleshooting

If you're experiencing issues integrating Pieces MCP with Continue.dev:

1. **Verify PiecesOS Status**: Ensure [PiecesOS is actively running](/products/core-dependencies/pieces-os/troubleshooting) on your system.

2. **Use Agent Mode**: MCP tools do not appear in regular chat—you must be in **agent mode**.

3. **YAML Parse Error**: Check indentation; YAML is whitespace-sensitive.

4. **Type Value**: Use `streamable-http` (with hyphen), not `streamableHttp` or `http`.

5. **Server Not Connecting**: Check the PiecesOS port (39300-39333) and URL format.

***

You're now set to enhance your Continue.dev workflow with powerful context retrieval through Pieces MCP. Happy coding!
