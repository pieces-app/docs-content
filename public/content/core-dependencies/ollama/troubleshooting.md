---
title: Ollama | Troubleshooting
path: /core-dependencies/ollama/troubleshooting
visibility: PRIVATE
status: PUBLISHED
description: Read documentation on basic Ollama troubleshooting steps below if you're experiencing connectivity issues between the Ollama client and PiecesOS. You can also find minimum and recommended device specifications for running local LLMs below.
metaTitle: Troubleshooting Ollama
metaDescription: Read documentation on basic Ollama troubleshooting steps below if you're experiencing connectivity issues between the Ollama client and PiecesOS.
---

## Initial Checks

PiecesOS uses Ollama as a wrapper for running local large language models, which allows developers to experiment with local models while leveraging PiecesOS features.

However, issues may arise from configuration mismatches, dependency updates, or environmental factors. 

For starters, make sure your machine meets the minimum system specifications and you have the latest version of PiecesOS and Ollama.

* **System Requirements:** Confirm your machine meets the minimum hardware and software requirements for running Ollama and your selected language model.

* **Latest Version:** Make sure you are using the latest version of both PiecesOS and Ollama.

<Callout type="info">
  Simple updates often resolve known bugs.
</Callout>

## Common Issues & Fixes

If Ollama fails to install or update, or if you encounter any dependency errors during installation, try the following steps to resolve the issue(s):

* **Verify Dependencies:** Ensure all required libraries and tools are installed on your system. Refer to the installation guide for the list of prerequisites.

* **Reinstall:** Uninstall any previous version of Ollama and perform a clean installation.

* **Network Issues:** If downloading fails, check your internet connection or proxy settings.

* **Error Messages:** Look for specific error messages during installation and consult the <a target="_blank" href="https://github.com/ollama/ollama/blob/main/docs/faq.md">Ollama FAQ</a> or official installation troubleshooting docs for guidance.

### Performance Problems

When running PiecesOS and using local models for generative AI use, you may experience slow response times or high CPU and RAM usage that causes your overall system to slow down.

You may need to:

* **Switch to Cloud Models:** You may need to acquire or switch over to a device with more RAM, a newer CPU with more cores, or a dedicated GPU with more VRAM.

* **Use a Lighter Model:** You may need to use a parameterized or more lightweight model if available.

* **Cut Down Instances:** If you are running multiple instances or flooding the LLM with queries and prompts, reduce the number of concurrent processes.

## Using Local Models

Older devices, regardless of operating system, may struggle to meet the hardware demands of heavy-duty LLMs, even with Ollama's streamlined setup.

### Minimum System Requirements

Local models demand more from your system than their cloud-hosted counterparts.

To ensure a stable, responsive experience—make sure your device fits these general minimum device specifications, pulled from Ollama documentation and other experience-tested public sources.

<Steps>
  <Step title="Operating System">
    Ollama is supported on macOS, Windows, and Linux devices—but you need to make sure your operating system is running at the correct minimum version to avoid compatibility issues.

    * **macOS:** macOS 11.0 (Big Sur) or later.

    * **Windows:** Windows 10 or later.

    * **Linux:** Ubuntu 18.04 or later.
  </Step>

  <Step title="RAM">
    Your system should have a minimum amount of RAM depending on the local model you’re trying to run.

    More RAM may further improve performance and reduce bottlenecks.

    * **3B Models:** 8GB of RAM

    * **7B Models:** 16GB of RAM

    * **13B Models:** 32GB of RAM
  </Step>

  <Step title="CPU">
    If your system doesn’t have a dedicated or otherwise capable GPU, running a CPU-tuned model may be in your best interests.

    * **Recommended:** Any modern CPU with at least 4 cores.

    * **13B Models:** Any modern CPU with at least 8 cores.
  </Step>

  <Step title="GPU">
    While you don’t need a GPU to run a local Ollama model as long as the LLM is CPU-tuned, a GPU can significantly speed up inference and the training of custom models.

    * **Recommended:** Any modern GPU with at least 6GB of VRAM.
  </Step>

  <Step title="Storage Space">
    Local large language models can occupy significant disk space, so ensure you have enough capacity for both the core installation and any custom models you plan to download or train.

    * **Minimum:** At least 12GB of free storage space for installing Ollama and other base models.

    * **Additional Storage:** Required for larger models that have additional dependencies
  </Step>
</Steps>

### Choosing the Right Model

Pick a model that fits your system's capabilities and performance limits, especially if you're using an older or less powerful device.

* **Lightweight Models:** Choose smaller or **quantized models** if you're using older hardware or have limited VRAM. Quantized models use less memory, making them easier to run without greatly affecting output quality for general tasks.

* **GPU-Tuned Models:** If you have a powerful GPU with enough VRAM, GPU-accelerated models usually run faster and deliver results more efficiently.

* **CPU-Tuned Models:** If you don't have a dedicated GPU or have low GPU memory, CPU-tuned models are a good alternative. Though slower, they can still offer reliable performance.

### Local Model Crashing

If you encounter 'hanging' or crashing issues when trying to run Pieces with a local LLM, it might be due to your system's hardware.

Insufficient system resources like RAM or VRAM can cause hiccups, slowdowns, and other glitches.

Here are some troubleshooting options:

1. **Check Hardware:** Ensure you have enough RAM, VRAM, and CPU capacity as recommended by the model.

2. **Update Drivers:** Use `vulkaninfo` (or a similar tool) to check for GPU or Vulkan-related errors if you have a Vulkan-based GPU. Update your GPU drivers if you find compatibility issues.

3. **Model Switching:** If you experience crashes or slowdowns, try switching to a less resource-intensive local model. Reducing complexity can help stabilize performance.

If you've tried all these troubleshooting steps but still face crashes, hanging, or other instabilities, you may need to switch to a cloud-based LLM.

### Vulkan-based GPUs

NVIDIA and AMD both use the Vulkan API framework in their GPUs, but there are known issues when using Vulkan GPUs for AI and LLM-focused tasks. For instance, a corrupted or outdated Vulkan API can lead to crashes.

If you encounter this problem, check Vulkan health in your terminal or command line by scanning for errors or warning messages. If any issues are found, **update your GPU drivers.**

### Checking Vulkan

To check your Vulkan health status, run `vulkaninfo` in your terminal or command line and look for errors or warnings.

### Updating GPU Drivers

If issues are detected, update your GPU drivers to ensure Vulkan compatibility and stability.