---
title: What is PiecesOS?
path: /core-dependencies/pieces-os
visibility: PUBLIC
status: PUBLISHED
description: PiecesOS is the background service that powers the entire Pieces ecosystem—running local AI models, managing Long-Term Memory, and connecting your tools via MCP.
metaTitle: What is PiecesOS? | Pieces Docs
metaDescription: Learn about PiecesOS, the background service that powers Long-Term Memory, on-device AI, and MCP integrations across the Pieces ecosystem.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/pieces_os.png"
---

## What is PiecesOS?

**PiecesOS** is a background service that runs on your machine. It orchestrates local data processing, manages on-device machine learning models, and serves as the bridge between your workflow and every Pieces product—including the [Pieces Desktop App](/products/desktop/onboarding), [MCP integrations](/products/mcp), and the [CLI](/products/cli).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/piecesos_bridging_all_products.png" alt="PiecesOS bridging all Pieces products and services" align="center" fullwidth="true" />

> PiecesOS bridging all Pieces products and services

## What PiecesOS Does

PiecesOS powers three core capabilities:

### Agentic Long-Term Memory (LTM-2.7)

The [LTM-2.7 Engine](/products/core-dependencies/pieces-os/long-term-memory) continuously captures workflow context—code you copy, screens you view, audio you hear—and stores it **locally on your device**. This memory powers [Timeline](/products/desktop/timeline), [Conversational Search](/products/desktop/conversational-search) (Agentic Chats), and [Single-Click Summaries](/products/desktop/single-click-summaries) (Agentic Summaries) with real context from your day.

The agent reasons across your memory in multiple turns, following threads, cross-referencing context, and building complete answers instead of one-shot guesses. It can search your memories, the web, your calendar, local files, and browser history automatically.

### Local & Cloud AI Models

PiecesOS manages AI model inference for all Pieces products. Run models **entirely on-device** for privacy, use **cloud models** (OpenAI, Anthropic, Google) for speed, or use **blended mode** for a mix of both. Configure your processing mode from the [Quick Menu](/products/core-dependencies/pieces-os/quick-menu#ml-processing).

### MCP Support

The [Model Context Protocol (MCP)](/products/mcp) is an open framework that lets LLMs access your workflow context. PiecesOS serves as the MCP host, connecting tools like Cursor, VS Code, Claude, and ChatGPT to your Long-Term Memory without custom integrations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/cursor_change_documentation_from_conversation_2_agentic_demo_screenshot.png" alt="Pieces MCP integration with Cursor for context-aware changes" align="center" fullwidth="true" />

> Pieces MCP integration with Cursor showing context-aware documentation changes

## Privacy & Local-First Design

All data captured by PiecesOS is stored **locally on your device**. Nothing leaves your machine unless you explicitly enable cloud features. PiecesOS applies on-device ML to filter out sensitive information and secrets.

<Callout type="info">
  Processing depends on your model choice: **Local** runs entirely on-device. **Blended** and **Cloud** send context to cloud providers. We're **SOC 2 Type II** certified and never use your data to train models. [Learn more about privacy and on-device storage.](/products/core-dependencies/on-device-storage)
</Callout>

## Installing PiecesOS

PiecesOS installs automatically with the [Pieces Desktop App](/products/desktop/onboarding). If you want to run it standalone (for example, with MCP integrations only), see [Manual Installation](/products/core-dependencies/pieces-os/manual-installation).

***

## Explore PiecesOS

<FancyCard title="Agentic LTM Engine" href="/products/core-dependencies/pieces-os/long-term-memory" colored={false}>
  Learn about Agentic Long-Term Memory, the agent toolbox, and how to enable, pause, and control memory capture.
</FancyCard>

<FancyCard title="Quick Menu" href="/products/core-dependencies/pieces-os/quick-menu" colored={false}>
  Manage PiecesOS settings, LTM, MCP, ML processing, and updates from the menu bar or system tray.
</FancyCard>

<FancyCard title="On-Device Storage" href="/products/core-dependencies/on-device-storage" colored={false}>
  Where Pieces stores your data locally, how to find logs, and how to back up or reset your database.
</FancyCard>

<FancyCard title="Troubleshooting" href="/products/core-dependencies/pieces-os/troubleshooting" colored={false}>
  Fix common installation issues, check system specs, update PiecesOS, and find logs on macOS, Windows, and Linux.
</FancyCard>
