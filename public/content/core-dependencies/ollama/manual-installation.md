---
title: Ollama | Manual Installation
path: /core-dependencies/ollama/manual-installation
visibility: PRIVATE
status: PUBLISHED
description: Read documentation on manually installing Ollama outside of the Pieces Desktop App for use with PiecesOS.
metaTitle: Ollama | Manual Installation
metaDescription: Read documentation on manually installing Ollama outside of the Pieces Desktop App for use with PiecesOS.
---

## Manual Installation Guide

Ollama is an *optional* dependency that enables local AI inference for Pieces Copilot and other AI-powered features in Pieces.

If you prefer to run LLMs on-device instead of using cloud-based AI, you will need to install Ollama manually.

This guide will walk you through the download, installation, and verification process for Ollama across Windows, macOS, and Linux.

## Minimum Version Requirement

PiecesOS requires a **specific minimum version** of Ollama to ensure compatibility, which is **0.5.5.**

Always install the latest stable release.

## Download Ollama

Visit the <a target="_blank" href="https://ollama.com/download">official Ollama website</a> to download the latest version, then install using the platform-specific instructions below.

<Tabs>
  <TabItem title="macOS">
    **Ollama | macOS Installation**

    Follow the steps below to manually install Ollama for your macOS device.

    1. Download the **macOS installer (**`.pkg`**)** from the <a target="_blank" href="https://ollama.com/download">Ollama website.</a>

    2. Double-click the `.pkg` file and follow the installation steps.

    3. After installation, verify the setup in **Terminal** by running `ollama --version`.
  </TabItem>

  <TabItem title="Windows">
    **Ollama | Windows Installation**

    Follow the steps below to manually install Ollama for your Windows device.

    1. Download the **Windows installer (.exe)** from the <a target="_blank" href="https://ollama.com/download">Ollama website.</a>

    2. Double-click the installer to launch the setup.

    3. Follow the on-screen instructions, accepting any security prompts.

    4. Once installed, open **Command Prompt** and verify the installation by running `ollama --version`.
  </TabItem>

  <TabItem title="Linux">
    **Ollama | Linux Installation**

    Follow the steps below to manually install Ollama for your Linux device.

    1. Open a terminal window and run `curl -fsSL https://ollama.ai/install sh | sh`.

    2. If using a package manager, manually install it with `sudo apt update && sudo apt install ollama`.

    3. Verify the installation with `ollama --version`.
  </TabItem>
</Tabs>

### Verify Ollama Integration

Once installed, ensure PiecesOS can detect and use Ollama.

1. Open the **Pieces Quick Menu** from your system tray or menu bar.

2. Navigate to `ML Processing`.

3. If Ollama is installed and recognized, it will appear under `Local AI Models`.

If it does not appear, restart PiecesOS and try again.

If PiecesOS **still doesn’t detect Ollama**, refer to [troubleshooting.](/products/core-dependencies/ollama/troubleshooting)

### Update Ollama

To update or uninstall Ollama on macOS or Windows, you can either download the latest version from the official Ollama website, update it through the Pieces Desktop App (if installed) or update it directly from the background Ollama process on your device.

For Linux, open your terminal and run `sudo apt update && sudo apt upgrade ollama`.

## Uninstall Ollama

If you no longer need local AI models or wish to remove the Ollama wrapper from your system, follow the instructions below specific to your platform.

<Tabs>
  <TabItem title="macOS">
    **Ollama | macOS Uninstallation**

    1. Open your terminal and run `sudo rm -rf /[username]/local/bin/ollama`.
  </TabItem>

  <TabItem title="Windows">
    **Ollama | Windows Uninstallation**

    1. Open `Settings`, navigate to `Apps`, then to `Installed Apps`.

    2. Search for `Ollama` and left-click the three dots next to the installed Ollama client, and click `Uninstall`.

    3. Restart your device to complete the uninstallation process.
  </TabItem>

  <TabItem title="Linux">
    **Ollama | Linux Uninstallation**

    1. Open your terminal and run `sudo apt remove ollama`.
  </TabItem>
</Tabs>

## Next Steps

You can read documentation about what [local LLMs are currently available](/products/core-dependencies/ollama/supported-models) on Ollama and are supported by PiecesOS, or [click here for troubleshooting](/products/core-dependencies/ollama/troubleshooting) if you’re experiencing installation issue.