---
title: Installation Guide | macOS
path: /meet-pieces/macos-installation-guide
visibility: PUBLIC
status: PUBLISHED
description: The following guide will help you install and run both PiecesOS and the Pieces Desktop Application quickly and easily.
metaTitle: Get started | MacOS
metaDescription: Get started with Pieces on macOS – install, configure, troubleshoot and optimize your setup for seamless AI-powered development.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_macos_install.webp"
---

<install-guide-buttons />

<Embed
  src="https://youtu.be/0uRNa8maMiA"
  title="How to set up Pieces on macOS"
/>



***

## Recommended Installation Method

Click the **buttons below** to download Pieces for your macOS device.

<CardGroup cols={2}>
  <Card title="Download — Pieces Desktop App (ARM)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/pieces_for_x/dmg-arm64/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_dmg_arm" gaPlatform="macos">
    *macOS 13.0 (Ventura) or higher required*
  </Card>

  <Card title="Download — Pieces Desktop App (Intel)" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/intel.png" href="https://builds.pieces.app/stages/production/pieces_for_x/dmg/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_dmg_intel" gaPlatform="macos">
    *macOS 13.0 (Ventura) or higher required*
  </Card>
</CardGroup>

<Callout type="alert">
  PiecesOS is a required Core Dependency. After you move Pieces Desktop to your Applications folder and open it for the first time, you'll be guided through installing PiecesOS automatically.
</Callout>

## Install the DMG

Once you've downloaded the correct `.dmg` file, it's time to install the Pieces Desktop App.

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

There are <mark>(2)</mark> requirements for installing Pieces on your macOS device:

1. Compatible OS Version—**macOS 13.0 (Ventura) or higher**

2. Compatible installer for your device's architecture—**Apple Silicon (ARM) or Intel**

Click here for a quick guide on [determining your OS type](/products/meet-pieces/troubleshooting/macos#checking-os-version), and here for [how to check your device's CPU architecture.](/products/meet-pieces/troubleshooting/macos#checking-cpu-type)

***

| **Component**      | **Minimum**                                                                   | **Recommended**                      | **Notes**                                                        |
| ------------------ | ----------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------- |
| *CPU*              | Any modern CPU                                                                | Multi-core CPU                       | Avoid dual-core processors—aim for at least a 4-core CPU.        |
| *RAM (Local Mode)* | 8 GB total system RAM with 2 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running locally.                        |
| *RAM (Cloud Mode)* | 8 GB total system RAM with 1 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running in cloud mode.                  |
| *Disk Space*       | 2 GB minimum (1 GB for PiecesOS + 0.5–1 GB for data), with at least 4 GB free | 8 GB with at least 6 GB free or more | Ensure additional free space for data storage and future growth. |

***

## Alternative Installations

If you cannot use the `.dmg` installer for any reason, you can install PiecesOS and the Pieces Desktop App using `.pkg` files or by using `Homebrew` through your Mac's terminal.

### via PKG (Apple Silicon / M-Series / ARM)

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App (PKG / ARM)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd-arm64/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_pkg_arm" gaPlatform="macos">
    macOS 13.0 (Ventura) or higher required.
  </Card>
</CardGroup>

### via PKG (Intel)

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App (PKG / Intel)" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/intel.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_pkg_intel" gaPlatform="macos">
    macOS 13.0 (Ventura) or higher required.
  </Card>
</CardGroup>

### Install the PKG

Once you've downloaded the correct `.pkg` file, it's time to install the Pieces Desktop App.

<Steps>
  <Step title="Find the download">
    Open your **Downloads** folder (or wherever you saved the installer) and look for the `.pkg` file you just downloaded.
  </Step>

  <Step title="Run the installer">
    Double-click the `.pkg` file to launch the installer wizard.
  </Step>

  <Step title="Follow the prompts">
    Click through the on-screen prompts—review the license agreement and enter your administrator password when prompted.
  </Step>

  <Step title="Complete the installation">
    Once the installer finishes, click `Close`. The Pieces Desktop App and PiecesOS are now installed in your **Applications** folder and ready to use.
  </Step>
</Steps>

## Install Using Homebrew

Alternatively, you may opt to install Pieces via Homebrew in your terminal.

<Card title="Installing via Homebrew" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/homebrew.png">
  You can install the Pieces Desktop App manually using Homebrew from your device's terminal.

  To do so:

  1. Ensure Homebrew is installed on your system.

  2. Copy and run the command below:

  ```bash
  brew install --cask pieces
  ```

  This command installs both the Pieces Desktop App and PiecesOS cask. If prompted, enter your administrator password.

  3. Wait for installation to complete—Homebrew will download and install the necessary files.

  Once it's done, you'll see a message indicating successful installation.
</Card>

## Post-Installation Tips

Read the documentation below for some tips and information to make sure you're up and running with the latest version(s) of PiecesOS and the Pieces Desktop App, as well as steps to uninstall Pieces software from your Apple device.

### Updating

The Pieces Desktop App automatically downloads and installs new updates.

You can also manually check for updates to PiecesOS and the Pieces Desktop App by hovering over your username in the top left, then hovering over `Update` and selecting either `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/macos/macos_check_pfd_for_updates_profile_dropdown.gif" alt="Checking for updates via the profile dropdown on macOS" align="center" fullwidth="true" />

### Uninstalling

On your macOS device, navigate to **Finder,** then select **Applications.**

Scroll or search until you find both `Pieces` and `PiecesOS.` Right-click on these two applications and select `Move to Trash`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/macos/macos_how_to_uninstall_pfd.gif" alt="Uninstalling Pieces from macOS Applications folder" align="center" fullwidth="true" />

## Additional Resources

Click here for additional [documentation on troubleshooting](/products/meet-pieces/troubleshooting/macos) or reach out to [support.](/products/support)
