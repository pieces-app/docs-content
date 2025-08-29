---
title: PiecesOS | Manual Installation
path: /core-dependencies/pieces-os/manual-installation
visibility: PUBLIC
status: PUBLISHED
description: Find standalone download links for PieceOS that match your system’s operating system (OS) or architecture, or download PiecesOS automatically with the Pieces Desktop App.
metaTitle: PiecesOS | Manual Installation
metaDescription: Find standalone download links for PieceOS that match your system’s operating system (OS) or architecture, or download PiecesOS automatically with the Pieces Desktop App.
---

## Installing PiecesOS

To get started, you’ll need to make sure your device is compatible with Pieces and has the minimum device recommendations.

## System Requirements

For macOS, Windows, and Linux devices, we recommend meeting these minimum device specifications:

***

| **Minimum**          | **Recommended**        | **Additional Information**                                                                                               |
| -------------------- | ---------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Any modern CPU       | A multi-core CPU       | PiecesOS supports multithreading for different operations and processes, making it faster the more CPU cores it can use. |
| 8GB of RAM           | 16GB+ of RAM           | At least 1GB of free RAM if running in cloud mode, or 2GB if running in local mode.                                      |
| 6GB of storage space | 10GB+ of storage space | At least 2GB for PiecesOS and the Pieces Desktop App with at least 4GB of free space for LTM data.                       |

***

PiecesOS and the Pieces Desktop App are lightweight, but you want to ensure you’ve got at least the above specifications to ensure a seamless user experience.

### Checking OS Version

PiecesOS is designed for macOS, Windows, and Linux, so you have the power of Pieces are your fingertips regardless of your device’s operating system.

<Callout type="alert">
  For Linux users, please note that PiecesOS is tested and currently compatible with Ubuntu 22+ and other Ubuntu-based distributions **only.**
</Callout>

Still, you need to be running a minimum version of that OS to ensure compatibility.

***

| **macOS**                       | **Windows**                   | **Linux**  |
| ------------------------------- | ----------------------------- | ---------- |
| macOS 12.0 (Monterey) or higher | Windows 10 (v.1809) or higher | Ubuntu 22+ |

***

If you need help determining your device’s OS version or system specifications, [read this documentation on the Troubleshooting page.](/products/core-dependencies/pieces-os/troubleshooting#common-installation-issues)

## Why Install PiecesOS Manually?

PiecesOS is installed by default when installing the Pieces Desktop App as a core dependency, but it can be installed manually for use with a Pieces plugin or extension if you’re not ready to dive into the entire Pieces ecosystem.

LTM, Pieces Drive, and Pieces Copilot will still be available to you.

### Installing via Pieces Desktop App

If you want to install PiecesOS automatically alongside the Pieces Desktop App, you can check out [these installation guides.](/products/desktop/download)

## Manual Download & Installation

There are different ways to install PiecesOS as a standalone entity, separate from the Pieces Desktop App.

To install, download the appropriate link for your device’s OS and architecture (if using a macOS device) and open the file, then walk through the guided installation steps as necessary.

## Windows

Click the download buttons below to install PiecesOS via `.exe` or `.appinstaller`.

<CardGroup cols={2}>
  <Card title="Download — Windows (.exe)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/os_server/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *Windows 10 (1809) or higher*
  </Card>

  <Card title="Download — Windows (.appinstaller)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/appinstaller/os_server.appinstaller?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *Windows 10 (1809) or higher*
  </Card>
</CardGroup>

### Updating PiecesOS (AppInstaller)

Note that currently, updating PiecesOS if installed via the `.appinstaller` (currently the *Recommended* installation method) files requires that you **quit the Pieces Desktop App**, then proceed with updating PiecesOS.

If this fails, make sure that the Pieces Desktop App is fully quit, as well as PiecesOS—then relaunch PiecesOS and proceed to download and install the update.

## macOS

Click the download buttons below to install PiecesOS for your ARM or Intel-based macOS device, or use the Homebrew instructions below.

<CardGroup cols={2}>
  <Card title="Download — ARM (.DMG)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/os_server/dmg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *macOS 12.0 (Monterey) or higher*
  </Card>

  <Card title="Download — Intel (.DMG)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/os_server/dmg/download?download=true&product=DOCUMENTATION_WEBSITE&ga_visitor=286281413.1724689222">
    *macOS 12.0 (Monterey) or higher*
  </Card>
</CardGroup>

<Card title="Installing via Homebrew" image="/assets/icons/platform_logos/macos_logo.png">
  You can also install PiecesOS manually using Homebrew from your device’s terminal.

  To do so:

  1. Ensure Homebrew is installed on your system.

  2. Run `brew install --cask pieces-os` in your terminal to install the Pieces `brew` package.
</Card>

## Linux

There are (2) requirements that must be met to download and install PiecesOS on your Linux device.

1. **Snap Support:** Ensure `snapd` is installed and enabled on your system. Most recent Ubuntu releases include `snapd` by default. If needed, install `snapd` by following official `snapd` documentation.

2. **Administrator Access:** You’ll need `sudo` privileges to install `snap` packages.

<Card title="Download — Linux" image="/assets/icons/platform_logos/ubuntu_logo.png">
  *Ubuntu 22+ required.*

  ***

  Run these commands **in order** to install and properly set up PiecesOS.

  1. **Open Terminal:** Open the Command-Line Interface (CLI) using `ctrl+alt+t`.

  2. Run `sudo snap install pieces-os` to install PiecesOS. You will be prompted to enter your local account’s password.

  3. Enter and run `sudo snap connect pieces-os:process-control :process-control` to enable offline and on-device machine learning and LLM functionality.

  4. To launch the PiecesOS, type `pieces-os` in your terminal and press `enter`.
</Card>

## Uninstalling PiecesOS

Select your operating system below to platform-specific steps to uninstalling PiecesOS.

<Tabs>
  <TabItem title="macOS">
    **On macOS Devices**

    On your macOS device, navigate to **Finder,** then select **Applications.**

    Scroll or search until you find `PiecesOS.` Right-click on these two applications and select `Move to Trash`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/macos/macos_how_to_uninstall_pfd.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    **On Windows Devices**

    Open **Settings,** then find **Apps** and search `Pieces.`

    The **PiecesOS application** will appear after that query. Click the three dots to the right of the application title, and click `Uninstall`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/windows/uninstalling_on_windows.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    **On Linux Devices**

    Uninstallation of PiecesOS on Linux is done via the CLI.

    To remove **PiecesOS,** type `sudo snap remove pieces-os` and press `enter`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/uninstall_pfd_from_terminal.png" alt="" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

## Troubleshooting

If you’re experiencing issues related to the manual installation of PiecesOS, see the [troubleshooting guide](/products/core-dependencies/pieces-os/troubleshooting#piecesos--troubleshooting) for quick fixes or access the [support page](/products/support) for helpful resources.

<Callout type="info">
  Want to install PiecesOS automatically with the Pieces Desktop App? [Click here.](/products/core-dependencies/pieces-os/manual-installation#installing-via-pieces-desktop-app)
</Callout>