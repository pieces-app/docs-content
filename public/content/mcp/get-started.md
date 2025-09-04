---
title: Get Started with Pieces MCP
path: /mcp/get-started
visibility: PUBLIC
status: PUBLISHED
description: Learn about Model Context Protocol (MCP) tools and discover how Pieces integrates the Long-Term Memory Engine (LTM-2.7) into your favorite IDEs and code editors.
metaTitle: Introducing Pieces Model Context Protocol (MCP) | Pieces Docs
metaDescription: Learn how Pieces Model Context Protocol (MCP) provides relevant workflow context to various IDE integrations. Explore the benefits of MCP for developers and teams.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/MCP/mcp.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/introducing_pieces_mcp/mcp.png" alt="" align="center" fullwidth="true" />

***

## Introducing Pieces Model Context Protocol (MCP)

Welcome to Pieces Model Context Protocol (MCP), an innovative way to connect Large Language Models (LLMs) to the context they need from your digital world.

## What is an MCP?

*Model Context Protocol*, or MCP, is an open standard developed by Anthropic that enables LLMs, like Claude and ChatGPT, to access external data sources and tools without needing complex, custom integrations.

In a way, MCP is becoming a *universal* context provider that uses a well-standardized communication protocol to pass information (like external data) or tools to LLM-powered applications.

For developers, this is extremely useful—because it means somebody using the Cursor agentic chat system can rope in external context to the LLM, giving it additional context outside of the purview of the active file or codebase they’re working in.

## How Pieces Integrates with MCP

The core of the Pieces ecosystem is [PiecesOS](/products/core-dependencies/pieces-os), which powers the Pieces Desktop App, browser extensions, and IDE plugins.

At its heart is the advanced [Long-Term Memory Engine (LTM-2.7)](/products/core-dependencies/pieces-os#ltm-25), which captures, enriches, and locally stores valuable contextual information from your daily workflow, such as code snippets, browser history, notes, and application data.

Pieces leverages the MCP to connect your favorite development tools and AI applications—like Cursor and GitHub Copilot—directly to PiecesOS, enabling smooth, context-rich interactions [entirely on your device.](/products/privacy-security-your-data#data-storage--control)

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/introducing_pieces_mcp/mcp-diagram.png" alt="" align="center" fullwidth="true" />

### Required Dependency

PiecesOS is a required dependency—you won’t be able to use Pieces as an MCP without it.

Read [documentation on PiecesOS](/products/core-dependencies/pieces-os) or jump to the [PiecesOS installation guides](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation) to get started.

## Use Cases and Benefits

Discover some critical use cases and benefits to using the Pieces MCP integration as a core tool alongside your daily development process.

### Context-Rich Debugging

Imagine encountering a tricky bug within [Cursor](/products/mcp/cursor).

Instead of manually reviewing logs or searching online, MCP allows Cursor to directly query Pieces LTM:

***

| **Prompt**                                                                                             | **Outcome**                                                                                                          |
| ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------- |
| *"Did the team decide to make* `enrichmentLevel` *case-sensitive for the applets? Is that the issue?"* | Cursor retrieves relevant team discussions and code decisions from PiecesOS, clarifying case-sensitivity decisions.  |
| *"Show me log entries from the recent API outages related to token expiration."*                       | Cursor fetches specific API outage logs and token-related errors stored by Pieces LTM for quick diagnosis.           |
| *"Have I previously encountered memory leaks in similar Node.js background tasks?"*                    | Cursor accesses your historical debugging notes and previous Node.js fixes saved in PiecesOS to suggest solutions.   |
| *"What configuration changes were made right before database latency spiked yesterday afternoon?"*     | Cursor gathers recent configuration modifications from PiecesOS to identify the exact changes affecting performance. |

***

### Contextual Queries

When integrated with [GitHub Copilot](/products/mcp/github-copilot), MCP enhances your coding experience by providing context-specific suggestions and history-driven recommendations:

***

| **Prompt**                                                                    | **Outcome**                                                                               |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| *“Show me previous implementations of this authentication method.”*           | Copilot fetches related past implementations from your Pieces LTM history.                |
| *“Show me similar code snippets to this React component.”*                    | Copilot retrieves related React components from your Pieces LTM history.                  |
| *“What fixes have I previously implemented for this type of database error?”* | Copilot accesses historical database error resolutions stored in Pieces LTM.              |
| *“Have I encountered this bug before?”*                                       | Copilot identifies past occurrences and corresponding fixes from your Pieces LTM context. |

***

## Why Developers Love Pieces MCP

Pieces MCP empowers developers to leverage personal context for AI-driven interactions, significantly reducing manual research, accelerating troubleshooting, and enhancing productivity.

By connecting directly to [PiecesOS](/products/core-dependencies/pieces-os), your context becomes a powerful, personalized source of truth that informs AI interactions:

* **Personalized Context**—The LLM understands your work based on real-time and historical data.

* **Secure and Local**—All data stays local for your [privacy and security.](/products/privacy-security-your-data)

* **Extensible and Open**: Easily integrate new tools and data sources with minimal effort.

***

*Pieces MCP —> Cursor*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/introducing_pieces_mcp/cursor_example_chat.png" alt="" align="center" fullwidth="true" />

***

## Technical Reference

Learn about the foundational layers of MCP architecture and the Pieces → MCP → LLM output flow you can achieve with the Pieces MCP integration.

### MCP Architecture

Pieces MCP consists of three main components that communicate via MCP for dynamic, secure context retrieval.

* **Host:** An AI-powered application (e.g., Cursor, Visual Studio Code).

* **Client:** Connectors embedded within the host, facilitating communication.

* **Server:** Small programs linking to specific tools or data sources, like PiecesOS and the `ask_pieces_ltm` tool.

### Pieces MCP Flow

Let’s take a look at the Pieces + MCP flow as you’d experience it in a familiar development environment:

<Steps>
  <Step title="Prompting">
    User sends a prompt via an AI tool (e.g., [Cursor](/products/mcp/cursor)).
  </Step>

  <Step title="Connecting the Dots">
    The MCP client within Cursor identifies relevant context servers (PiecesOS).
  </Step>

  <Step title="Gathering Context">
    The MCP server fetches relevant data from Pieces LTM-2.7.
  </Step>

  <Step title="Generating the Output">
    Context is returned and utilized by the AI to respond effectively, and the LLM provides a context-rich response.
  </Step>
</Steps>

***

*Pieces MCP —> GitHub Copilot*

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/mcp_documentation/introducing_pieces_mcp/visualstudio_example_chat.png" alt="" align="center" fullwidth="true" />

***

## Getting Started

Explore how quickly MCP enhances your productivity by delivering deep, personalized context directly to your AI-driven coding flow.

To begin using Pieces MCP, [install and launch PiecesOS](/products/core-dependencies/pieces-os/manual-installation) on your system, then follow our integration documentation for setting up the MCP server within your favorite IDE:

* [Pieces MCP + Cursor Integration Guide](/products/mcp/cursor)

* [Pieces MCP + GitHub Copilot Integration Guide](/products/mcp/github-copilot)

* [Pieces MCP + Goose Integration Guide](/products/mcp/goose)

***

## What's Next?

The MCP ecosystem continues to expand rapidly, with more integrations and tools on the horizon.

Join the community, build your custom MCP servers, and transform how AI assists your everyday tasks.

<Callout type="tip">
  Stay tuned for more detailed guides, examples, and tutorials coming soon.
</Callout>

Happy Coding!