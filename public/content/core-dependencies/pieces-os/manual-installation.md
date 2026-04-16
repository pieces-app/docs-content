---
title: Manual Installation
path: /core-dependencies/pieces-os/manual-installation
visibility: PUBLIC
status: PUBLISHED
description: Download and install PiecesOS as a standalone service for macOS, Windows, or Linux—for use with MCP integrations or without the Pieces Desktop App.
metaTitle: Manual Installation | PiecesOS
metaDescription: Download and install PiecesOS manually on macOS, Windows, or Linux. Includes system requirements, download links, Homebrew and Snap instructions, and uninstall steps.
---

## When to Install Manually

PiecesOS installs automatically with the [Pieces Desktop App](/products/desktop/onboarding). Install it manually if you want to use [Pieces MCP integrations](/products/mcp) without the full Desktop experience—LTM, Conversational Search, and MCP features still work.

## System Requirements

| **Minimum** | **Recommended** | **Notes** |
| --- | --- | --- |
| Any modern CPU | Multi-core CPU | PiecesOS supports multithreading |
| 8 GB RAM | 16 GB+ RAM | 1 GB free (cloud mode) or 2 GB free (local mode) |
| 6 GB storage | 10 GB+ storage | ~2 GB for PiecesOS + at least 4 GB for LTM data |

### Minimum OS Versions

| **macOS** | **Windows** | **Linux** |
| --- | --- | --- |
| macOS 12.0 (Monterey)+ | Windows 10 (v.1809)+ | Ubuntu 22+ |

<Callout type="info">
  Need help checking your specs or OS version? See [Troubleshooting](/products/core-dependencies/pieces-os/troubleshooting#checking-system-specifications).
</Callout>

***

## Windows

<CardGroup cols={2}>
  <Card title="Download — Windows (.exe)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/os_server/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *Windows 10 (1809) or higher*
  </Card>

  <Card title="Download — Windows (.appinstaller)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/appinstaller/os_server.appinstaller?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *Windows 10 (1809) or higher*
  </Card>
</CardGroup>

<Callout type="alert">
  **Installation path:** Avoid **OneDrive**, **iCloud Drive**, and other cloud-synced locations—use a local drive (the default path is recommended).
</Callout>

## macOS

<CardGroup cols={2}>
  <Card title="Download — ARM (.DMG)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/os_server/dmg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *macOS 12.0 (Monterey) or higher*
  </Card>

  <Card title="Download — Intel (.DMG)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/os_server/dmg/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *macOS 12.0 (Monterey) or higher*
  </Card>
</CardGroup>

### Installing via Homebrew

```bash
brew install --cask pieces-os
```

## Linux

<Callout type="alert">
  PiecesOS on Linux requires **Ubuntu 22+** and **snapd** enabled on your system.
</Callout>

<Steps>
  <Step title="Open Terminal">
    Press `ctrl+alt+t` to open your terminal.
  </Step>

  <Step title="Install PiecesOS">
    Run `sudo snap install pieces-os` and enter your password when prompted.
  </Step>

  <Step title="Enable local ML">
    Run `sudo snap connect pieces-os:process-control :process-control` to enable on-device machine learning and LLM functionality.
  </Step>

  <Step title="Launch PiecesOS">
    Type `pieces-os` and press Enter.
  </Step>
</Steps>

***

## Uninstalling PiecesOS

<Tabs>
  <TabItem title="macOS">
    Open **Finder** > **Applications**. Find `PiecesOS`, right-click, and select `Move to Trash`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/macos/macos_how_to_uninstall_pfd.gif" alt="Uninstalling PiecesOS from macOS Applications folder" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    Open **Settings** > **Apps**, search for `Pieces`. Click the three dots next to PiecesOS and select `Uninstall`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/windows/uninstalling_on_windows.gif" alt="Uninstalling PiecesOS from Windows Settings" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    Run `sudo snap remove pieces-os` in your terminal.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/uninstall_pfd_from_terminal.png" alt="Uninstalling PiecesOS from the Linux terminal" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

***

Having trouble? See [Troubleshooting PiecesOS](/products/core-dependencies/pieces-os/troubleshooting) or visit the [Support page](/products/support).
