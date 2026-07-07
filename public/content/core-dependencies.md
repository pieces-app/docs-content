---
title: Core Dependencies
path: /core-dependencies
visibility: PUBLIC
status: PUBLISHED
description: PiecesOS powers the Pieces ecosystem—Desktop App, MCP integrations, and on-device memory. Learn about core dependencies and how PiecesOS works.
metaTitle: Core Dependencies for Pieces | PiecesOS Guide
metaDescription: PiecesOS powers the Desktop App and MCP integrations, capturing and storing your context on-device. Learn setup and dependencies.
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/core_dependencies.png" alt="Core dependencies overview banner" align="center" fullwidth="true" />


## What Are Core Dependencies?

Pieces products, including the [Pieces Desktop Application](/products/desktop), are built on [PiecesOS](/products/core-dependencies/pieces-os), which provides a local, secure, and efficient experience with built-in AI capabilities.

## What Is PiecesOS?

To run any Pieces software, you will need **PiecesOS,** the backbone of the Pieces Suite. This lightweight application runs in the background of your device.

It powers the [Long-Term Memory (LTM-2.7) Engine](/products/core-dependencies/pieces-os#ltm-27) and [Conversational Search](/products/desktop/conversational-search). [Pieces Drive](/products/desktop/drive) is a **legacy** material manager retained for existing workflows; LTM and [Timeline](/products/desktop/timeline) replace it for new users.

**PiecesOS**: The backbone of the Pieces suite, managing local memory, AI-driven workflow enhancements, [Pieces MCP](/products/mcp), and other integrations within your development environment.

## On-Device Processing

PiecesOS runs directly on your device and powers core Pieces capabilities without sending your data to the cloud:

- **Long-Term Memory (LTM-2.7)** workflow capture and processing
- **Code enrichment** and analysis
- **Secret detection** and security scanning
- **Metadata and tag generation**

Capture, indexing, and storage happen entirely on your device through PiecesOS. AI features that need a large language model—like [Conversational Search](/products/desktop/conversational-search)—send only scoped, relevant context to a cloud model for that request.

## What Does PiecesOS Do?

PiecesOS is a lightweight service that handles everything from on-device context capture and storage to coordinating AI-assisted workflows.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/pfd_x_piecesos_and_ollama.png" alt="Pieces Desktop App and PiecesOS architecture" align="center" fullwidth="true" />

PiecesOS is **required** for all Pieces products, including:

* Pieces Desktop App

* [MCP integrations](/products/mcp) for [JetBrains IDEs](/products/mcp/jetbrains-ides), [VS Code](/products/mcp/vs-code), [Raycast](/products/mcp/raycast), and [many other tools](/products/mcp), plus [the Pieces CLI](/products/cli).

## Why Do We Need PiecesOS?

Pieces is designed with **speed and efficiency** in mind, so PiecesOS acts as the central hub between different Pieces products to minimize client-side overhead and additional code while also being secure and highly configurable.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/performance_privacy_flexibility.png" alt="PiecesOS performance, privacy, and flexibility benefits" align="center" fullwidth="true" />

Our focus on **security and flexibility** is why PiecesOS does as much as possible on your device. By keeping capture and storage local, the user experience benefits from:

* **100% local memory storage** with full control over data.

* **Scoped cloud requests**, so only the relevant context for a given prompt is ever sent to an AI model.

* **Lightweight, background operation**, consuming minimal system resources.

This is especially useful in enterprise settings where strong device security is important.

***

| **Dependency** | **Purpose**                                                           | **Required?**                                   |
| -------------- | --------------------------------------------------------------------- | ----------------------------------------------- |
| *PiecesOS*     | Manages memory, developer material storage, and MCP client communication, capturing and storing your context on-device. | Yes — this is required for all Pieces products. |

***
