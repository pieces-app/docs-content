---
title: Cross-Platform Issues
path: /meet-pieces/troubleshooting/cross-platform
visibility: PUBLIC
status: PUBLISHED
description: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected, regardless of your operating system.
metaTitle: Cross-platform issues | Pieces Docs
metaDescription: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected, regardless of your operating system.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_troubleshooting_cross_platform.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/cross_platform/troubleshooting_multiOS.png" alt="" align="left" fullwidth="true" />

***

## Basic Troubleshooting

Find links to detailed sections on specific troubleshooting steps as well as information on choosing between cloud and local models, system requirements, and more.

<on-device-storage />

## Versions & Updates

Many issues can stem from out-of-date plugins, extensions, Ollama, the Pieces Desktop App, or PiecesOS itself.

### Updating PiecesOS

Both PiecesOS and the Pieces Desktop Application update automatically if installed through the Pieces Suite Installer.

For standalone installations (non-macOS/Linux store-based), updates are checked daily or upon application launch, prompting you to install or delay.

See your specific OS page for platform-specific instructions on updating PiecesOS:

* [macOS](/products/meet-pieces/troubleshooting/macos#updating-piecesos)

* [Windows](/products/meet-pieces/troubleshooting/windows#updating-piecesos)

* [Linux](/products/meet-pieces/troubleshooting/linux#updating-piecesos)

### Updating the Pieces Desktop App

Ensuring the Desktop App is up-to-date is critical.

See your specific OS page for platform-specific update instructions on updating the Pieces Desktop App:

* [macOS](/products/meet-pieces/troubleshooting/macos#updating-the-pieces-desktop-app)

* [Windows](/products/meet-pieces/troubleshooting/windows#updating-the-pieces-desktop-app)

* [Linux](/products/meet-pieces/troubleshooting/linux#updating-the-pieces-desktop-app)

## Connection Issues with PiecesOS

You may occasionally encounter connection issues with PiecesOS or your Personal Cloud, resulting in:

* Pieces Copilot not generating outputs

* Difficulty finding saved materials

* Trouble sharing code snippets

The quickest way to resolve this basic connection issue is to restart PiecesOS, then check for updates.

### Restarting PiecesOS & Checking Updates

To restart and check for updates to PiecesOS:

1. Restart PiecesOS

2. Ensure PiecesOS is running (look for the Pieces Icon in your system tray or menu bar)

3. Check for and install available updates

4. Verify that the Pieces Desktop Application and the plugin or extension you are attempting to use is up-to-date

## Common Installation Issues

Common issues can occur when setting up PiecesOS and the Pieces Desktop App for the first time.

Platform-specific solutions are detailed on their respective OS pages:

* [macOS](/products/meet-pieces/troubleshooting/macos#common-installation-issues)

* [Windows](/products/meet-pieces/troubleshooting/windows#common-installation-issues)

* [Linux](/products/meet-pieces/troubleshooting/linux#common-installation-issues)

## Using Local Models

Running Pieces software with a local LLM through **Ollama** can offer greater privacy, faster responses (when properly configured), and independence from cloud dependencies.

By utilizing the Ollama framework, users can efficiently deploy and manage local language models tailored to their needs.

However, local models often require robust hardware configurations and careful optimization to run smoothly.

Older devices, regardless of operating system, may struggle to meet the hardware demands of these LLMs, even with Ollama's streamlined setup.

### Minimum System Requirements

Local models demand more from your system than their cloud-hosted counterparts.

To ensure a stable, responsive experience—make sure your device fits these general minimum device specifications, pulled from Ollama documentation and other experience-tested public sources.

<Steps>
  <Step title="Operating System">
    Ollama is supported on macOS, Windows, and Linux devices—but you need to make sure your operating system is running at the correct minimum version to avoid compatibility issues.

    * **macOS:** macOS 13.0 (Ventura) or higher

    * **Windows:** Windows 10 or higher

    * **Linux:** Ubuntu 22+ or higher
  </Step>

  <Step title="RAM">
    Your system should have a minimum amount of RAM depending on the local model you’re trying to run. More RAM may further improve performance and reduce bottlenecks.

    * **3B Models:** 8GB of RAM

    * **7B Models:** 16GB of RAM

    * **13B Models:** 32GB of RAM
  </Step>

  <Step title="CPU">
    If your system doesn’t have a dedicated or otherwise capable GPU, running a CPU-tuned model may be in your best interests.

    * **Recommended:** Any modern CPU with at least 4 cores

    * **13B Models:** Any modern CPU with at least 8 cores
  </Step>

  <Step title="GPU">
    While you don’t need a GPU to run a local Ollama model as long as the LLM is CPU-tuned, a GPU can significantly speed up inference and the training of custom models.

    * **Recommended:** Any modern GPU with at least 6GB of VRAM
  </Step>

  <Step title="Disk Space">
    Local large language models can occupy significant disk space, so ensure you have enough capacity for both the core installation and any custom models you plan to download or train.

    * **Minimum:** At least 12GB of free storage space for installing Ollama and other base models.

    * **Additional Storage:** Required for larger models that have additional dependencies
  </Step>
</Steps>

### Minimum System Requirements for Pieces Software

Your device, regardless of platform, should meet the following basic system specifications for using Pieces software.

<pos-pfd-system-reqs />

### Choosing the Right Model

Select a model that matches your system’s capabilities and performance limitations, especially if you’re running an older or weaker device.

* **Lightweight Models:** Opt for smaller or **quantized models** if you’re using older hardware or have limited VRAM. Quantized models are optimized to reduce memory usage, making them easier to run without significantly impacting output quality for general tasks.

* **GPU-Tuned Models:** If you have a strong GPU with enough VRAM, GPU-accelerated models often run faster and produce results more efficiently.

* **CPU-Tuned Models:** If you lack a dedicated GPU or have low GPU memory, CPU-tuned models are a fallback option. Although slower, they can still provide consistent performance.

### Local Model Crashing

If you are running into ‘hanging’ or crashing issues when attempting to power Pieces using a local LLM, it may be because of your system’s hardware.

Insufficient system resources, like RAM or VRAM may cause hiccups, slowdowns, and other glitches.

There are a few options available to you for troubleshooting:

1. **Check Hardware:** Verify that you have sufficient RAM, VRAM, and CPU headroom as recommended by the model.

2. **Update Drivers:** Run `vulkaninfo` (or a similar tool) to check for GPU or Vulkan-related errors, if you have a Vulkan-based GPU. Update your GPU drivers if you detect compatibility issues.

3. **Model Switching:** If you experience crashes or slowdowns, try switching to a less resource-intensive local model. Reducing complexity can stabilize performance.

If you’ve tried all of these troubleshooting steps but are still experiencing crashes, hanging-time, or other instabilities, you may need to switch to a cloud-based LLM.

## Vulkan-based GPUs

NVIDIA and AMD both utilize the Vulkan API framework in their GPUs, but there are known issues with using Vulkan GPUs for AI and LLM-centered workloads.

For example, a corrupted or outdated Vulkan API can cause crashes.

If you are experiencing this issue, you can check Vulkan health in your terminal or command line and scanning for errors or warning message—if there are any issues detected, **update your GPU drivers.**

### Checking Vulkan

To check your Vulkan health status, run `vulkaninfo` in your terminal or command line and look for errors or warnings.

### Updating GPU Drivers

If issues are detected, update your GPU drivers to ensure Vulkan compatibility and stability.

## Checking Hardware

It may be necessary to verify your system’s specifications if you experience ongoing issues.

See the OS-specific pages for instructions on how to check CPU, RAM, and GPU details:

* [macOS](/products/meet-pieces/troubleshooting/macos#checking-cpu-type)

* [Windows](/products/meet-pieces/troubleshooting/windows#checking-hardware-specifications)

* [Linux](/products/meet-pieces/troubleshooting/linux#checking-system-information)