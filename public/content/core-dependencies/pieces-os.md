---
title: What is PiecesOS?
path: /core-dependencies/pieces-os
visibility: PUBLIC
status: PUBLISHED
description: PiecesOS is the background service powering Pieces—capturing on-device memory, coordinating AI models, and connecting tools via MCP.
metaTitle: What is PiecesOS? | Pieces Docs
metaDescription: Learn about PiecesOS, the background service that powers Long-Term Memory, on-device capture, and MCP integrations across the Pieces ecosystem.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/pieces_os.png"
---

<Callout type="alert">
  **Action required:** Cloud services no longer work on PiecesOS versions prior to 12.4.0 (deprecated June 5th 2026). Update to 12.4.0 or later to restore Chat, Work Summaries, and Single Click Summaries.
</Callout>

## What is PiecesOS?

**PiecesOS** is a background service that runs on your machine. It orchestrates on-device data capture and storage, coordinates AI model requests, and serves as the bridge between your workflow and every Pieces product—including the [Pieces Desktop App](/products/desktop/onboarding), [MCP integrations](/products/mcp), and the [CLI](/products/cli).

<piecesos-bridge-diagram />

## What PiecesOS Does

PiecesOS powers three core capabilities:

### Agentic Long-Term Memory (LTM-2.7)

The [LTM-2.7 Engine](/products/core-dependencies/pieces-os/long-term-memory) continuously captures workflow context—code you copy, screens you view, audio you hear—and stores it **locally on your device**. This memory powers [Timeline](/products/desktop/timeline), [Conversational Search](/products/desktop/conversational-search) (Agentic Chats), and [Single-Click Summaries](/products/desktop/single-click-summaries) (Agentic Summaries) with real context from your day.

The agent reasons across your memory in multiple turns, following threads, cross-referencing context, and building complete answers instead of one-shot guesses. It can search your memories, the web, your calendar, local files, and browser history automatically.

### AI Models

PiecesOS coordinates AI model requests for all Pieces products. Choose from four model families—Claude, Gemini, Grok, and ChatGPT—each available in Fast, Balanced, and Extra Thinking modes. See [Choose a Model](/products/desktop/conversational-search/models) to pick a family and mode.

### MCP Support

The [Model Context Protocol (MCP)](/products/mcp) is an open framework that lets LLMs access your workflow context. PiecesOS serves as the MCP host, connecting tools like Cursor, VS Code, Claude, and ChatGPT to your Long-Term Memory without custom integrations.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/pieces_os_main/cursor_change_documentation_from_conversation_2_agentic_demo_screenshot.png" alt="Pieces MCP integration with Cursor for context-aware changes" align="center" fullwidth="true" />

> Pieces MCP integration with Cursor showing context-aware documentation changes

## Privacy & Local-First Design

All data captured by PiecesOS is stored **locally on your device**. Capture, indexing, and storage happen on-device, and PiecesOS applies on-device ML to filter out sensitive information and secrets.

<Callout type="info">
  AI features that need a large language model run in the cloud, where only the scoped context for that request is sent—the rest of your data stays on your machine. We're **SOC 2 Type II** certified and never use your data to train models. [Learn more about privacy and on-device storage.](/products/core-dependencies/on-device-storage)
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
