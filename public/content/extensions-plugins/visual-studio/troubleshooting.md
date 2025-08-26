---
title: Troubleshooting
path: /extensions-plugins/visual-studio/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: This page guides you on how to fix common issues with the Pieces for Visual Studio Extension and how to connect with the Pieces support team or community.
metaTitle: Troubleshooting Common Issues in Pieces for Visual Studio Extension
metaDescription: Fix issues with the Pieces for Visual Studio Plugin using troubleshooting steps designed for quick and easy resolutions.
---

# Having Issues with Visual Studio?

Read the documentation below for a series of basic troubleshooting steps you can take if the Pieces for Visual Studio Extension isn’t working as expected.

<on-device-storage />

## Quick Checks

Many issues stem from an out-of-date version of PiecesOS or a system inadequately powered to run local models. Find out more below.

### Ensure You Have the Latest Versions

First, ensure you're using the latest version of the <a target="_blank" href="https://marketplace.visualstudio.com/items?itemName=MeshIntelligentTechnologiesInc.PiecesVisualStudio">Pieces for Visual Studio Extension</a> from the Visual Studio Marketplace and the newest version of [PiecesOS](/products/core-dependencies/pieces-os). The minimum supported version is Visual Studio 2022 — 17.9.0 or higher.

### Check the Settings for Pieces

It's common for users to adjust a setting in Pieces for Visual Studio that leads to unexpected actions. Double-check your [configuration](/products/extensions-plugins/visual-studio/configuration) to ensure everything is set as you expect.

### PiecesOS

PiecesOS and the Pieces Desktop Application update automatically if installed through the Pieces Suite Installer.

For standalone installations (non-macOS/Linux store-based), updates are checked daily or upon application launch, prompting you to install or delay.

See your specific OS page for platform-specific instructions on updating PiecesOS:

* [macOS](/products/meet-pieces/troubleshooting/macos#updating-piecesos)

* [Windows](/products/meet-pieces/troubleshooting/windows#updating-piecesos)

* [Linux](/products/meet-pieces/troubleshooting/linux#updating-piecesos)

### Minimum System Requirements for Pieces Software

Regardless of platform, your device should meet the following basic system specifications for using the Pieces for Developers software.

***

| **Component**      | **Minimum**                                                                   | **Recommended**                      | **Notes**                                                        |
| ------------------ | ----------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------- |
| *CPU*              | Any modern CPU                                                                | Multi-core CPU                       | Avoid dual-core processors—aim for at least a 4-core CPU.        |
| *RAM (Local Mode)* | 8 GB total system RAM with 2 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running locally.                        |
| *RAM (Cloud Mode)* | 8 GB total system RAM with 1 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running in cloud mode.                  |
| *Disk Space*       | 2 GB minimum (1 GB for PiecesOS + 0.5–1 GB for data), with at least 4 GB free | 8 GB with at least 6 GB free or more | Ensure additional free space for data storage and future growth. |

***

## Checking Hardware

It may be necessary to verify your system’s specifications if you experience ongoing issues.

See the OS-specific pages for instructions on how to check CPU, RAM, and GPU details:

* [macOS](/products/meet-pieces/troubleshooting/macos#checking-cpu-type)

* [Windows](/products/meet-pieces/troubleshooting/windows#checking-hardware-specifications)

* [Linux](/products/meet-pieces/troubleshooting/linux#checking-system-information)

### Restart Visual Studio After Updates

If you’ve recently installed or updated PiecesOS or the Pieces for Visual Studio Extension, restart the IDE.

Contact the <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#docs-vscode">Pieces support team</a> if the issue still persists.

### Refreshing Copilot Chats

You might need to restart or refresh the Pieces Copilot chat, especially if you're using a cloud LLM and lose your WiFi connection.

This can sometimes cause the LLM to hang, appearing to generate a response but eventually timing out or getting stuck in a loop.

To fix this, click the **three vertical dots** in the top-right corner of your Copilot Chat window and select `Refresh`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/troubleshooting/refresh_copilot_chat.png" alt="" align="center" fullwidth="true" />