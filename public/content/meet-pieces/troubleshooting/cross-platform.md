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

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/cross_platform/troubleshooting_multiOS.png" alt="Cross-platform troubleshooting banner" align="left" fullwidth="true" />

***

## Basic Troubleshooting

Find links to detailed sections on specific troubleshooting steps as well as information on system requirements and more.

<on-device-storage />

## Versions & Updates

Many issues can stem from out-of-date MCP integrations, the Pieces Desktop App, or PiecesOS itself.

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

* Conversational Search not generating outputs

* Difficulty finding saved materials

* Trouble sharing code snippets

The quickest way to resolve this basic connection issue is to restart PiecesOS, then check for updates.

### Restarting PiecesOS & Checking Updates

To restart and check for updates to PiecesOS:

1. Restart PiecesOS

2. Ensure PiecesOS is running (look for the Pieces Icon in your system tray or menu bar)

3. Check for and install available updates

4. Verify that the Pieces Desktop Application and the MCP integration you are attempting to use is up-to-date

## Common Installation Issues

Common issues can occur when setting up PiecesOS and the Pieces Desktop App for the first time.

Platform-specific solutions are detailed on their respective OS pages:

* [macOS](/products/meet-pieces/troubleshooting/macos#common-installation-issues)

* [Windows](/products/meet-pieces/troubleshooting/windows#common-installation-issues)

* [Linux](/products/meet-pieces/troubleshooting/linux#common-installation-issues)

## System Requirements

Your device, regardless of platform, should meet the following basic system specifications for using Pieces software.

<pos-pfd-system-reqs />

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