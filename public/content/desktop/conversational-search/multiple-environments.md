---
title: Use Conversational Search in IDEs
path: /desktop/conversational-search/multiple-environments
visibility: PUBLIC
status: PUBLISHED
description: Use Conversational Search across IDEs and tools—primarily via MCP—with Long-Term Memory and PiecesOS.
metaTitle: Use Conversational Search in IDEs | Pieces Docs
metaDescription: Use Conversational Search across MCP-enabled IDEs and productivity tools with PiecesOS and Long-Term Memory context.
---

## Use Conversational Search in IDEs

Pieces connects to popular IDEs, editors, and productivity tools—most often through **Model Context Protocol (MCP)**—so you can use the same workflow in the environment you prefer.

## Cross-environment access

Editor integrations today run primarily through **MCP** (see the [Integrations overview](/products/integrations-overview)). Legacy editor **plugins** are retired; use the MCP guides for current setup.

In supported environments you get **PiecesOS** and **Long-Term Memory** context alongside **Conversational Search**. Legacy **Pieces Drive** remains available where documented; new workflows should use **LTM** and **Timeline**.

### MCP and editor guides

| **Environment** | **Documentation** |
| ------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
| [JetBrains IDEs](/products/mcp/jetbrains-ides) | Setup for JetBrains via MCP |
| [Visual Studio Code](/products/mcp/vs-code) | VS Code via MCP |
| [GitHub Copilot in Visual Studio](/products/mcp/github-copilot) | Visual Studio via MCP |
| [Other editors (MCP hub)](/products/mcp) | Raycast, notebooks, and additional MCP hosts |
| Browser | [Web Extension](/products/web-extension) |
| Neovim | [Neovim plugin](https://pieces.app/plugins/neovim) (external) |

Additionally:

* [Pieces CLI](/products/cli)
* [Raycast (MCP)](/products/mcp/raycast)
* [Obsidian](/products/obsidian)

## Integration with other applications

In IDEs that use the Pieces **Applet** or MCP, you get a familiar chat experience with context-aware suggestions tied to your project. **LTM** preferences and model choices stay aligned with the Desktop App where supported.

### Shared conversation threads

Conversational Search supports **cross-threading**: chat history and context can move between the Desktop App and other connected environments so you can continue the same thread.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Other%20Environments/pieces_cross_threading.png" alt="Cross-threaded Conversational Search chat shared between Desktop App and IDE" align="center" fullwidth="true" />

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/copilot_in_environment_demo_part_two.png" alt="Continuing a Conversational Search conversation across environments" align="center" fullwidth="true" />

## The Pieces user experience

Core behavior—chat history, context controls, and LLM configuration—is designed to feel consistent across environments.

### Flutter-supported environments

On platforms such as JetBrains IDEs, Visual Studio Code, and the Pieces Web Extension, a Flutter-based **Applet** delivers a standardized experience for Conversational Search and related tools.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/pieces_web_extension_copilot_applet.png" alt="Conversational Search applet in the Web Extension" align="center" fullwidth="true" />

### Custom UI environments

Where a Flutter applet is not available (for example some editors or the CLI), the UI is tailored to the host while keeping the same capabilities.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/pieces_copilot_sublime_text.png" alt="Conversational Search interface in Sublime Text" align="center" fullwidth="true" />

***

## Next Steps

Return to the Desktop-focused guides when you configure memory, context, and models in the app:

[Talk with Your Memories →](/products/desktop/conversational-search/using-conversational-search)
