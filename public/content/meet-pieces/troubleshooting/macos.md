---
title: Issues | macOS
path: /meet-pieces/troubleshooting/macos
visibility: PUBLIC
status: PUBLISHED
description: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected on your macOS device.
metaTitle: Issues | macOS
metaDescription: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected on your Windows issues.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_troubleshooting_macOS.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/troubleshooting_macos.png" alt="" align="left" fullwidth="true" />

***

## Installation & Updating Fixes

PiecesOS and the Pieces Desktop App can be downloaded using several installation methods, and they can be updated differently depending on the method used.

You can also find information below on how to determine your Apple device's CPU architecture and OS version.

<on-device-storage />

## Manual Installation Methods

If you’re experiencing difficulties installing PiecesOS or the Pieces Desktop App, you can manually install both software by downloading the standalone files or using terminal commands.

<Callout type="alert">
  If you’re unsure which `.dmg` or `.pkg` you need based on your device’s CPU, [click here.](/products/meet-pieces/troubleshooting/macos#checking-cpu-type)
</Callout>

### via PKG Files

Make sure to select the correct Pieces `.pkg` for your macOS device—Apple Silicon (ARM) or Intel.

| **Apple Silicon (ARM)**                                                                                                                                                                                      | **Intel**                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a target="_blank" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd-arm64/download?download=true&product=DOCUMENTATION_WEBSITE">Download Pieces PKG for macOS (Apple Silicon / ARM)</a> | <a target="_blank" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd/download?download=true&product=DOCUMENTATION_WEBSITE">Download Pieces PKG for macOS (Intel)</a> |

### via DMG Files

Make sure to select the correct Pieces `.dmg` files for your macOS device—Apple Silicon (ARM) or Intel.

| **Apple Silicon (ARM)**                                                                                                                                                                  | **Intel**                                                                                                                                                                                         |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a target="_blank" href="https://builds.pieces.app/stages/production/os_server/dmg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE">Download PiecesOS DMG for macOS (ARM)</a> | <a target="_blank" href="https://builds.pieces.app/stages/production/os_server/dmg/download?download=true&product=DOCUMENTATION_WEBSITE">Download PiecesOS DMG for macOS (Intel)</a>              |
| [Download Pieces Desktop App DMG for macOS (ARM)](https://builds.pieces.app/stages/production/pieces_for_x/dmg-arm64/download?download=true\&product=DOCUMENTATION_WEBSITE)              | <a target="_blank" href="https://builds.pieces.app/stages/production/pieces_for_x/dmg/download?download=true&product=DOCUMENTATION_WEBSITE">Download Pieces Desktop App DMG for macOS (Intel)</a> |

### via Homebrew

A singular brew command, `brew install—- cask pieces`, automatically manages installing PiecesOS and the Pieces Desktop App.

## Versions & Updates

Many issues can stem from out-of-date plugins, extensions, the desktop app, or PiecesOS.

### Updating PiecesOS

To restart and check for updates to PiecesOS on macOS:

1. Restart PiecesOS

2. Ensure PiecesOS is running (look for the **Pieces Icon** in your system tray)

3. Check for and install available updates

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_piecesos_for_updates.gif" alt="" align="center" fullwidth="true" />

### Updating the Pieces Desktop App

Updating the **Pieces Desktop App** on Windows and macOS systems can be done by clicking the **user icon** to the right of the **search bar** at the top of the Pieces Desktop Window, then clicking `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

To check the Pieces Desktop App for updates on macOS:

1. Open the Pieces Desktop App

2. Click the **user icon** to the right of the **search bar** at the top of the main app view

3. Click `Check for Desktop App Updates`

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_check_pfd_for_updates_profile_dropdown.gif" alt="" align="center" fullwidth="true" />

You can also click `Check for PiecesOS Updates` as an alternative to doing so in from the PiecesOS system window in your taskbar.

## Common Installation Issues

There are a range of common install issues on Apple devices, like having an out-of-date OS version or selecting the wrong installation package.

### Checking OS Version

Pieces Suite applications require a minimum macOS version of **macOS 13.0 (Ventura).** If you’re experiencing installation issues, you should first check your OS version to make sure it’s up-to-date.

To determine your Apple device’s version of macOS:

1. Click the **Apple** icon in the top-left corner of your screen

2. Select `About This Mac`

3. Under your device name (i.e., MacBook Air), look for the last line on the list, titled `macOS`

The `macOS` line will report what version of macOS installed, e.g., `Sequoia 15.1.1`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_about_mac.gif" alt="" align="center" fullwidth="true" />

### Checking CPU Type

Intel and Apple Silicon (ARM) devices run on entirely separate CPU architectures, so downloading the wrong package for your Apple device can cause apps from the Pieces Suite to be rendered useless.

To determine what CPU architecture your Apple device utilizes:

1. Click the **Apple () icon** in the top-left corner of your screen.

2. Select **About This Mac**, and look for the **Overview section.** The first line will contain your CPU type:

* **Apple Silicon / ARM:** You will see an M-Series processor, e.g., `Apple M3`

* **Intel:** You will see an Intel processor, e.g., `2.6 GHz Intel Core i7`

Once you’ve determined your CPU architecture, [download the correct installation package accordingly.](/products/meet-pieces/macos-installation-guide#recommended-installation-method)

## Restart & Retry

If installation fails due to having an outdated version of macOS or installing the wrong package for your device’s architecture, restart your machine and try the installation again from scratch.

If the problem persists, please open a <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> for further assistance, or book a call with our engineers.
