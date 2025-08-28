---
title: Understanding Ollama
path: /core-dependencies/ollama
visibility: PUBLIC
status: PUBLISHED
description: Read about Ollama, an optional dependency which enables fully on-device generative AI capabilities between Pieces Drive and the Pieces Copilot.
metaTitle: Ollama | Pieces Core Dependancies
metaDescription: Read about Ollama, an optional dependency which enables fully on-device generative AI capabilities between Pieces Drive and the Pieces Copilot.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/ollama.png"
---

## What Is Ollama?

Ollama is an *optional* but powerful dependency that allows PiecesOS to run Large Language Models (LLMs) directly on your device instead of relying on cloud-based AI processing. 

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/ollama_core_dependencies.png" alt="" align="center" fullwidth="true" />

Unlike PiecesOS—which is required for all Pieces functionality—Ollama is only needed if you want to use local AI models with Pieces Copilot.

<Callout type="tip">
  Using Ollama for local generative AI is *a separate process* from how PiecesOS uses local, in-house LoRA models for processing data with the LTM-2.5 Engine.
</Callout>

## Why Use Ollama?

Ollama acts as a wrapper around `llama.cpp`, making local AI processing faster, more stable, and easier to use.

It simplifies model deployment and ensures compatibility with [Pieces for Developers’ supported LLMs](/products/core-dependencies/ollama/supported-models) and allows for new local models to be integrated soon after they are released.

Additionally, many developers and organizations prefer local LLMs over cloud-hosted models for reasons such as:

* **Stronger data security,** as it keeps proprietary code and sensitive queries 100% local.

* **Faster response times** with no network delays during generative AI processing and local inference.

* **Offline accessibility** for use even when no internet connection is present.

* **Enterprise compliance** so all AI queries remain within company-managed environments.

### How It Works

Ollama is integrated with PiecesOS to enable local modal inference and generative AI capabilities.

Here’s how Ollama works alongside PiecesOS:

* **Serves on-device LLMs**, reducing cloud dependency and enhancing privacy.

* **Automatically detects existing Ollama installations**, so if you’ve already installed it for other purposes, Pieces can use it without requiring a reinstallation.

* **Supports a curated set of models**, all using `Q4_K_S` quantization for performance optimization.

* **Ensures compatibility** with PiecesOS through minimum version requirements to avoid stability issues.

<Callout type="tip">
  Since Ollama is several GBs in size, it is **not installed by default**. Users must opt in during the PiecesOS setup process if they want local model support.
</Callout>

### Using Local vs Cloud Models

PiecesOS primarily uses cloud-based AI models for Pieces Copilot.

However, users who prefer on-device AI for speed, privacy, or offline access can install Ollama to enable local models. 

[You can read about the system requirements for Ollama here.](/products/core-dependencies/ollama/troubleshooting#using-local-models)

***

| **Feature**              | **Cloud AI (Default)**                                                                                      | **Local AI (Ollama)**                                  |
| ------------------------ | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| **Processing Location**  | Cloud-based (requires internet)                                                                             | On-device (runs locally)                               |
| **Performance**          | Dependent on internet speed                                                                                 | Potentially faster response times (no network latency) |
| **Data Privacy**         | Data only sent to cloud if included as context in a Copilot Chat—reverts on OpenAI, Gemini Privacy Policies | 100% local (no data transmission from local device)    |
| **Model Availability**   | Uses several cloud-hosted models                                                                            | Uses user-installed local models                       |
| **Storage Requirements** | Minimal outside of the PiecesOS installation                                                                | Several GBs (model storage)                            |
| **Offline Support**      | No                                                                                                          | Yes                                                    |

***
