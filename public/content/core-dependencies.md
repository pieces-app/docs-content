---
title: Core Dependencies
path: /core-dependencies
visibility: PUBLIC
status: PUBLISHED
description: Learn about PiecesOS, the core dependency that powers the Pieces Desktop App and the entire Pieces suite of plugins and extensions, including built-in local models for on-device AI.
metaTitle: Pieces Core Dependencies
metaDescription: Learn about PiecesOS, the core dependency that powers the Pieces Desktop App and the entire Pieces suite of plugins and extensions, including built-in local models for on-device AI.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/core_dependencies.png" alt="" align="center" fullwidth="true" />

***

## What Are Core Dependencies?

Pieces products, including the [Pieces Desktop Application](/products/desktop), are built on [PiecesOS](/products/core-dependencies/pieces-os), which provides a local, secure, and efficient experience with built-in AI capabilities.

## What Is PiecesOS?

To run any Pieces software, you will need **PiecesOS,** the backbone of the Pieces Suite. This lightweight application runs in the background of your device.

It powers the [Long-Term Memory (LTM-2.7) Engine](/products/core-dependencies/pieces-os#ltm-27), [Pieces Drive,](/products/desktop/drive) and the [Pieces Copilot.](/products/desktop/copilot)

**PiecesOS**: The backbone of the Pieces suite, managing local memory, AI-driven workflow enhancements, [Pieces MCP](/products/mcp/get-started), and other integrations within your development environment.

## Local Models

Pieces includes built-in local models that run directly through PiecesOS—no external dependencies required.

These models power:
- **Long-Term Memory (LTM-2.7)** workflow processing
- **Code enrichment** and analysis
- **Pieces Copilot** with on-device LLMs
- **Secret detection** and security scanning

All local processing happens entirely on your device through PiecesOS, ensuring privacy and offline functionality.

## What Does PiecesOS Do?

PiecesOS is a lightweight service that handles everything from local model management and context storage to advanced local inference for AI-assisted workflows.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/pfd_x_piecesos_and_ollama.png" alt="" align="center" fullwidth="true" />

PiecesOS is **required** for all Pieces products, including:

* Pieces Desktop App

* Plugins & Extensions for [JetBrains](/products/extensions-plugins/jetbrains), [VS Code](/products/extensions-plugins/visual-studio-code), [Sublime Text](/products/extensions-plugins/sublime), [JupyterLab](/products/extensions-plugins/jupyterlab), [Neovim](/products/extensions-plugins/neovim-plugin), [Raycast](/products/raycast), [Obsidian](/products/obsidian), [the Pieces CLI](/products/cli), and more.

## Why Do We Need PiecesOS?

Pieces is designed with **speed and efficiency** in mind, so PiecesOS acts as the central hub between different Pieces products to minimize client-side overhead and additional code while also being secure and highly configurable.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/performance_privacy_flexibility.png" alt="" align="center" fullwidth="true" />

Our focus on **security and flexibility** is why we've built local models directly into PiecesOS—users can work entirely with on-device generative AI, and by offloading most operations locally, the user experience benefits from:

* **Instant AI-powered assistance** without cloud latency.

* **100% local memory storage** with full control over data.

* **Offline functionality**, ensuring a seamless experience even when disconnected from the internet.

* **Lightweight, background operation**, consuming minimal system resources.

Local models are built into PiecesOS automatically, providing on-device AI capabilities without any additional setup or installation.

This is especially useful in enterprise settings where strong device security is important.

***

| **Dependency** | **Purpose**                                                           | **Required?**                                   |
| -------------- | --------------------------------------------------------------------- | ----------------------------------------------- |
| *PiecesOS*     | Manages memory, developer material storage, and plugin communication. Includes built-in local models for on-device AI. | Yes — this is required for all Pieces products. |

***
