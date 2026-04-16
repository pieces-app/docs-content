---
title: State of Plugins
path: /extensions-plugins/state-of-plugins
visibility: PUBLIC
status: PUBLISHED
description: Pieces IDE plugins and extensions have been sunset. All integration support is moving to the Model Context Protocol (MCP). Learn what changed and where to go next.
metaTitle: Pieces Plugins — Sunset Notice | Pieces Docs
metaDescription: Pieces is sunsetting individual IDE plugins in favor of standardized MCP integrations. Find out what this means and how to migrate.
---

## Pieces Plugins Have Been Sunset

Pieces is **no longer developing or supporting** individual IDE plugins and extensions. Most existing plugins have **stopped working** and will not receive further updates.

All integration support is moving to the **[Model Context Protocol (MCP)](/products/mcp)** — an open standard that lets any MCP-compatible tool connect to PiecesOS and your Long-Term Memory without a custom plugin.

<Callout type="alert">
  If you are currently using a Pieces plugin, it may already be non-functional. **Switch to the MCP integration** for your editor or tool as soon as possible.
</Callout>

## Why MCP?

- **One standard, many tools.** MCP is supported across Cursor, VS Code, JetBrains, Claude, ChatGPT, and [many more](/products/mcp).
- **No plugin maintenance.** You no longer need to install, update, or troubleshoot a separate plugin per editor.
- **Broader reach.** Any tool that speaks MCP can access Pieces Long-Term Memory, Pieces Drive, and the full Pieces toolset — today and in the future.

## What Should I Do?

<Steps>
  <Step title="Uninstall your Pieces plugin">
    Remove the Pieces extension from VS Code, JetBrains, Sublime Text, Neovim, JupyterLab, Visual Studio, or whichever editor you were using.
  </Step>
  <Step title="Set up PiecesOS and MCP">
    Follow the [MCP Getting Started guide](/products/mcp) to connect PiecesOS to your editor via MCP.
  </Step>
  <Step title="Find your editor's MCP page">
    We have dedicated setup guides for [Cursor](/products/mcp/cursor), [VS Code](/products/mcp/vs-code), [GitHub Copilot](/products/mcp/github-copilot), [JetBrains](/products/mcp/jetbrains-ides), [Claude Desktop](/products/mcp/claude-desktop), and [more](/products/mcp).
  </Step>
</Steps>

## Legacy Plugin Pages

The plugin docs below are kept for reference but describe **unsupported, non-functional** software. Do not rely on them for new setups.

- [VS Code Extension](/products/extensions-plugins/visual-studio-code)
- [JetBrains Plugin](/products/extensions-plugins/jetbrains)
- [Visual Studio Extension](/products/extensions-plugins/visual-studio)
- [JupyterLab Extension](/products/extensions-plugins/jupyterlab)
- [Sublime Text Plugin](/products/extensions-plugins/sublime)
- [Neovim Plugin](/products/extensions-plugins/neovim-plugin)

***

Questions? Visit our [support page](/products/support) or [get started with MCP](/products/mcp).
