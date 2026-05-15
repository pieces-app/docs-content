---
title: DMG Installation | macOS
path: /meet-pieces/macos-installation-guide/dmg
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for macOS using the DMG installer. The recommended method with support for both Apple Silicon and Intel Macs.
metaTitle: DMG Installation | macOS
metaDescription: Install Pieces via DMG on macOS. Download for Apple Silicon (M1/M2/M3/M4) or Intel, drag to Applications, and start using Pieces.
---

## DMG Installation (Recommended)

The DMG installer is the recommended method for installing Pieces on macOS. Choose the correct version for your Mac's processor.

<CardGroup cols={2}>
  <Card title="Download — Apple Silicon (ARM)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/pieces_for_x/dmg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_dmg_arm" gaPlatform="macos">
    *For M1, M2, M3, M4 Macs*

    macOS 13.0 (Ventura) or higher required.
  </Card>

  <Card title="Download — Intel" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/intel.png" href="https://builds.pieces.app/stages/production/pieces_for_x/dmg/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_dmg_intel" gaPlatform="macos">
    *For pre-2020 Macs*

    macOS 13.0 (Ventura) or higher required.
  </Card>
</CardGroup>

<Callout type="alert">
  PiecesOS is a required Core Dependency. After you move Pieces Desktop to your Applications folder and open it for the first time, you'll be guided through installing PiecesOS automatically.
</Callout>

### Install the DMG

<Steps>
  <Step title="Find the download">
    Open your **Downloads** folder (or wherever you saved the installer) and look for the `.dmg` file you just downloaded (e.g., `Pieces.dmg`).
  </Step>

  <Step title="Mount the DMG">
    Double-click the `.dmg` file to mount it.
  </Step>

  <Step title="Drag & Drop into Applications">
    Drag the application icon from the mounted `.dmg` window into your **Applications** folder.
  </Step>

  <Step title="Eject the DMG">
    Go back to **Finder**, right-click the mounted image, and select **Eject** to unmount it.
  </Step>
</Steps>

<Callout type="alert">
  Put Pieces in **Applications** or another **local** folder—not **iCloud Drive** or other synced locations.
</Callout>

### System Requirements

| **Component**      | **Minimum**                                                                   | **Recommended**                      | **Notes**                                                        |
| ------------------ | ----------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------- |
| *OS Version*       | macOS 13.0 (Ventura)                                                          | macOS 14.0 or higher                 | Apple Silicon or Intel processor.                                |
| *CPU*              | Any modern CPU                                                                | Multi-core CPU                       | Avoid dual-core processors—aim for at least a 4-core CPU.        |
| *RAM (Local Mode)* | 8 GB total system RAM with 2 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running locally.                        |
| *RAM (Cloud Mode)* | 8 GB total system RAM with 1 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running in cloud mode.                  |
| *Disk Space*       | 2 GB minimum (1 GB for PiecesOS + 0.5–1 GB for data), with at least 4 GB free | 8 GB with at least 6 GB free or more | Ensure additional free space for data storage and future growth. |

Click here for a quick guide on [determining your OS type](/products/meet-pieces/troubleshooting/macos#checking-os-version), and here for [how to check your device's CPU architecture](/products/meet-pieces/troubleshooting/macos#checking-cpu-type).

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [macOS troubleshooting](/products/meet-pieces/troubleshooting/macos) for common solutions.
