---
title: Understanding Local Models
path: /core-dependencies/local-models
visibility: PUBLIC
status: PUBLISHED
description: Learn about local models, an optional capability that enables fully on-device generative AI for Conversational Search.
metaTitle: Local Models | Pieces Core Dependencies
metaDescription: Learn about local models, an optional capability that enables fully on-device generative AI for Conversational Search.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/core_dependencies/ollama.png"
---

## What Are Local Models?

Local models are *optional* but powerful AI capabilities built into PiecesOS that allow you to run Large Language Models (LLMs) directly on your device instead of relying on cloud-based AI processing.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_dependencies_assets/figma_mockups/ollama_core_dependencies.png" alt="" align="center" fullwidth="true" />

Unlike cloud models—which require an internet connection—local models run entirely on your device, providing complete privacy and offline functionality.

<Callout type="tip">
  Local models for Conversational Search are *separate* from the in-house LoRA models that PiecesOS uses for processing data with the LTM-2.7 Engine. Those built-in models are always available and require no additional downloads.
</Callout>

## Why Use Local Models?

PiecesOS provides local AI processing directly through its built-in infrastructure, making it faster, more stable, and easier to use.

Local models can be downloaded on-demand and ensure compatibility with [Pieces supported LLMs](/products/core-dependencies/local-models/supported-models), allowing new local models to be integrated soon after they are released.

Additionally, many developers and organizations prefer local LLMs over cloud-hosted models for reasons such as:

* **Stronger data security**, as it keeps proprietary code and sensitive queries 100% local.

* **Faster response times** with no network delays during generative AI processing and local inference.

* **Offline accessibility** for use even when no internet connection is present.

* **Enterprise compliance** so all AI queries remain within company-managed environments.

### How It Works

Local models are integrated with PiecesOS to enable local model inference and generative AI capabilities.

Here's how local models work with PiecesOS:

* **Serve on-device LLMs**, reducing cloud dependency and enhancing privacy.

* **Download on-demand**, so you only install the models you need for your workflow.

* **Support a curated set of models**, all optimized for performance with efficient quantization.

* **Ensure compatibility** with PiecesOS through automatic version management.

<Callout type="tip">
  Since local models are several GBs in size, they are **not downloaded by default**. You can download them through the Conversational Search model selector when you need them.
</Callout>

### Using Local vs Cloud Models

PiecesOS supports both cloud-based and local AI models for Conversational Search.

Users who prefer on-device AI for speed, privacy, or offline access can download local models directly through PiecesOS.

Supported cloud providers and example models include:

- OpenAI: GPT-5.2 Pro, GPT-5.2, GPT-5.1, GPT-5 Thinking, GPT-5, GPT-5 Fast, o4 Mini, o3 Pro, o3 Mini, o3, o1, GPT-4.1, GPT-4o, GPT-4o Mini
- Anthropic: Claude 4.5 Opus, Claude 4.5 Sonnet, Claude 4.5 Haiku, Claude 4 Sonnet, Claude 3.7 Sonnet, Claude 3.5 Sonnet, Claude 3.5 Haiku
- Google: Gemini 3 Pro Preview, Gemini 3 Flash Preview, Gemini 2.5 Pro, Gemini 2.5 Flash, Gemini 2.5 Flash Lite, Gemini 2 Flash Lite

[See the full Cloud Models list →](/products/large-language-models/cloud-models)

***

| **Feature**              | **Cloud AI (Default)**                                                                                      | **Local AI**                                           |
| ------------------------ | ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| **Processing Location**  | Cloud-based (requires internet)                                                                             | On-device (runs locally)                               |
| **Performance**          | Dependent on internet speed                                                                                 | Potentially faster response times (no network latency) |
| **Data Privacy**         | Data only sent to cloud if included as context in a Conversational Search chat—governed by provider privacy policies | 100% local (no data transmission from local device)    |
| **Model Availability**   | Uses several cloud-hosted models                                                                            | Download models on-demand through PiecesOS             |
| **Storage Requirements** | Minimal outside of the PiecesOS installation                                                                | Several GBs (model storage)                            |
| **Offline Support**      | No                                                                                                          | Yes                                                    |

## Required Specifications

Local models use more system resources than cloud-based AI. To run local LLMs smoothly, your device should meet the following minimum specifications. These guidelines are based on Ollama documentation and experience-tested public sources such as [LocalLLM.in's VRAM requirements guide](https://localllm.in/blog/ollama-vram-requirements-for-local-llms).

### Minimum System Requirements

| **Component**        | **Minimum**                                                                 |
| -------------------- | --------------------------------------------------------------------------- |
| **Operating System** | macOS 11.0 (Big Sur) or later, Windows 10 or later, or Ubuntu 18.04 or later |
| **RAM**              | 8GB for 3B models; 16GB for 7B models; 32GB for 13B models                 |
| **CPU**              | Modern CPU with at least 4 cores (8 cores recommended for 13B models)       |
| **GPU (optional)**   | 6GB+ VRAM recommended for faster inference                                  |
| **Storage**          | At least 12GB free for Ollama and base models; more for larger models       |

### VRAM Guidelines by Model Size

If you use a dedicated GPU, the amount of VRAM you need depends on the model size and quantization. The following are general guidelines for running models at Q4_K_M quantization:

| **VRAM**     | **Typical model size**                          |
| ------------ | ----------------------------------------------- |
| **3–4 GB**   | 3–4B parameter models (e.g., 4k context)        |
| **6–8 GB**   | 7–9B models (e.g., Llama 3.1 8B, Qwen3 8B)     |
| **10–12 GB** | 12–14B models (e.g., Gemma 3 12B, Qwen3 14B)   |
| **16–24 GB** | 22–35B models (e.g., Gemma 3 27B, Qwen3 32B)  |
| **48 GB+**   | 70B+ models (e.g., Llama 3.3 70B, Qwen2.5 72B) |

Total VRAM usage includes model weights, KV cache (which grows with context length), and system overhead. For more precise requirements for a specific model, refer to [LocalLLM.in's Ollama VRAM requirements guide](https://localllm.in/blog/ollama-vram-requirements-for-local-llms).

***
