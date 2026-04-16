---
title: Conversational Search in Other Environments
path: /desktop/copilot/multiple-environments
visibility: PUBLIC
status: PUBLISHED
description: Use Conversational Search across IDEs and tools—primarily via MCP—with Long-Term Memory and PiecesOS.
metaTitle: Conversational Search in multi-environments | Pieces Docs
metaDescription: Use Conversational Search across MCP-enabled IDEs and productivity tools with PiecesOS and Long-Term Memory context.
---

## Using Conversational Search in IDEs

Pieces connects to several popular IDEs, editors, and productivity tools—most often through **Model Context Protocol (MCP)**—so you can use Pieces in the environment you prefer.

## Cross-Environment Access

Editor and IDE integrations today run primarily through **MCP** (see the [Integrations overview](/products/integrations-overview)). Legacy editor **plugins** are retired; use the MCP guides for current setup.

In supported environments you get **PiecesOS** and **Long-Term Memory** context alongside **Conversational Search**. Legacy **Pieces Drive** remains available where documented; new workflows should use **LTM** and **Timeline**.

### MCP & editor guides

Use the links below for current integration documentation.

***

| **Environment**                                                                          | **Documentation**                                                                            |
| ------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------- |
| [JetBrains IDEs](/products/mcp/jetbrains-ides)                                            | [GitHub Copilot in Visual Studio](/products/mcp/github-copilot)                            |
| [Other editors (MCP hub)](/products/mcp)                                                  | [Visual Studio Code](/products/mcp/vs-code)                                                  |
| Browser | [Web Extension](/products/web-extension) |
| <a target="_blank" href="https://pieces.app/plugins/neovim">Neovim</a>                     | [Jupyter & notebooks (MCP hub)](/products/mcp)                                             |

***

Additionally, find documentation here for our other productivity and collaboration tools:

* [Pieces CLI](/products/cli)

* [Raycast (MCP)](/products/mcp/raycast)

* [Obsidian](/products/obsidian)

## Integration with Other Applications

Conversational Search is available in several IDEs through **MCP** and, where documented, other integrations.

When you use Conversational Search within an IDE, you experience a similar chat interface with environments using the Pieces Applet view, complete with context-aware suggestions tailored to your current project.

The settings and configurations (such as LTM context and model preferences) remain consistent with the Desktop App, ensuring a seamless transition between environments.

### Shared Conversation Threads

The Conversational Search experience supports *cross-threading.*

This means that your chat history and contextual data can be shared between the Desktop App and other environments.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Other%20Environments/pieces_cross_threading.png" alt="Cross-threaded Conversational Search chat shared between Desktop App and IDE" align="center" fullwidth="true" />

Whether you start a conversation in the Desktop App and later continue it in an IDE, your context and settings persist—making for a fluid, uninterrupted workflow.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/copilot_in_environment_demo_part_two.png" alt="Continuing a Conversational Search conversation across environments" align="center" fullwidth="true" />

## The Pieces User Experience

Conversational Search is designed to maintain a consistent core experience—offering essential features like chat history, context management, and LLM configuration—across all environments.

### Flutter-Supported Environments

In platforms such as JetBrains, Visual Studio Code, and the Pieces Web Extension, Pieces leverages a dedicated Flutter-based *Applet* view which provides a standardized user experience for interacting with Conversational Search and the Pieces Drive.

***

*Pieces Web Extension*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/pieces_web_extension_copilot_applet.png" alt="Conversational Search applet in the Web Extension" align="center" fullwidth="true" />

***

### Custom UI Environments

For environments that do not support Flutter applets (e.g., Sublime Text or the CLI), Conversational Search adapts with a custom interface tailored to the specific platform.

Although the visual presentation differs, all core features remain available, so the learning curve is as minimal as possible while still providing Pieces functionalities.

***

*Pieces for Sublime Text Plugin*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/pieces_copilot/pieces_copilot_in_multiple_environments/pieces_copilot_sublime_text.png" alt="Conversational Search interface in Sublime Text" align="center" fullwidth="true" />

***
