---
title: Core Dependencies
path: /core-dependencies
visibility: PUBLIC
status: PUBLISHED
description: Learn about PiecesOS and Ollama, the two core dependencies that power the Pieces Desktop App and the entire Pieces  suite of plugins and extensions.
metaTitle: Pieces Core Dependencies
metaDescription: Learn about PiecesOS and Ollama, the two core dependencies that power the Pieces Desktop App and the entire Pieces suite of plugins and extensions.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/core_dependencies.png" alt="" align="center" fullwidth="true" />

***

## What Are Core Dependencies?

Pieces products, including the [Pieces Desktop Application](/products/desktop), utilize *two core dependencies* to provide a local, secure, and efficient experience—[PiecesOS](/products/core-dependencies/pieces-os) and [Ollama](/products/core-dependencies/ollama)**.**

## What Are They?

To run any Pieces software, you will need **\[1] PiecesOS,** the backbone of the Pieces Suite. This lightweight application runs in the background of your device.

It powers the [Long-Term Memory (LTM-2.7) Engine](/products/core-dependencies/pieces-os#ltm-27), [Pieces Drive,](/products/desktop/drive) and the [Pieces Copilot.](/products/desktop/copilot)

Running local LLMs requires downloading and installing the **\[2] Ollama** wrapper to power on-device AI capabilities, such as querying Pieces Copilot or the local inference required by the LTM-2.7 Engine.

1. **PiecesOS**: The backbone of the Pieces suite, managing local memory, AI-driven workflow enhancements, [Pieces MCP](/products/mcp/get-started), and other integrations within your development environment.

2. **Ollama**: A specialized wrapper that enables local AI inference, allowing Pieces Copilot and other features to leverage machine learning models *directly on your device.*

## What Do They Do?

These dependencies—**PiecesOS and Ollama**—are lightweight services and engines that handle everything from local model management and context storage to advanced local inference for AI-assisted workflows.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/pfd_x_piecesos_and_ollama.png" alt="" align="center" fullwidth="true" />

PiecesOS is **required** for all Pieces products, including:

* Pieces Desktop App

* Plugins & Extensions for [JetBrains](/products/extensions-plugins/jetbrains), [VS Code](/products/extensions-plugins/visual-studio-code), [Sublime Text](/products/extensions-plugins/sublime), [JupyterLab](/products/extensions-plugins/jupyterlab), [Azure Data Studio](/products/extensions-plugins/azure-data-studio), [Neovim](/products/extensions-plugins/neovim-plugin), [Raycast](/products/raycast), [Obsidian](/products/obsidian), [the Pieces CLI](/products/extensions-plugins/cli), and more.

## Why Do We Need Them?

Pieces is designed with **speed and efficiency** in mind, so PiecesOS acts as the end-all between different Pieces products to minimize client-side overhead and additional code while also being secure and highly configurable.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/performance_privacy_flexibility.png" alt="" align="center" fullwidth="true" />

Our focus on **security and flexibility** is why we’ve introduced the Ollama wrapper for local large language models—users can switch entirely to on-device generative AI, and by offloading most operations locally, the user experience benefits from:

* **Instant AI-powered assistance** without cloud latency.

* **100% local memory storage** with full control over data.

* **Offline functionality**, ensuring a seamless experience even when disconnected from the internet.

* **Lightweight, background operation**, consuming minimal system resources.

However, you don't have to install Ollama if you don't want to use it.

You can install it if you want to use local models, which is especially useful in enterprise settings where strong device security is important.

***

| **Dependency** | **Purpose**                                                           | **Required?**                                     |
| -------------- | --------------------------------------------------------------------- | ------------------------------------------------- |
| *PiecesOS*     | Manages memory, developer material storage, and plugin communication. | Yes — this is required for all Pieces products.   |
| *Ollama*       | Enables locally powered generative AI queries and model execution.    | No — but this is required for local AI inference. |

***