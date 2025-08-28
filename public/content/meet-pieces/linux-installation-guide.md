---
title: Installation Guide | Linux
path: /meet-pieces/linux-installation-guide
visibility: PUBLIC
status: PUBLISHED
description: The following guide will help you install and run both PiecesOS and the Pieces for Developers Desktop Application quickly and easily on your Linux device.
metaTitle: Get started | Linux
metaDescription: Get started with Pieces on Linux – install, configure, troubleshoot and optimize your setup for seamless AI-powered development.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_linux_install.png"
---

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1740162782513/1fdc656d-398c-4e69-ba4a-381c880fffe0.png" alt="" align="center" fullwidth="true" />

***

## Install Pieces for Linux

Follow the steps below to download and install Pieces for Linux using the Command-Line Interface (CLI).

### Requirements

There are several requirements that your Linux device must meet to download and install the Pieces Desktop App, PiecesOS, and *ensure LTM-2 compatibility.*

* **Snap Support:** Ensure `snapd` is installed and enabled on your system. Most recent Ubuntu releases include `snapd` by default. If needed, install `snapd` by following the official `snapd` documentation.

* **Administrator Access:** You’ll need `sudo` privileges to install `snap` packages.

* **Minimum OS Type:** PiecesOS has been tested and developed primarily for Ubuntu 22+ or later-based distributions, so make sure your system is updated to at least Ubuntu 22+ or later.

* **X11 Window Manager:** Virtual Linux machines or dedicated instances of Linux, even PiecesOS-compatible Ubuntu 22+ distributions, **must utilize X11** as the proprietary Window Manager.

<Callout type="tip">
  To determine which display manager your Linux device is using, go to **Settings,** then **System,** and **System Details** to see if you are using an X11 or a non-LLVM compatible manager.
</Callout>

<Card title="Download — Linux" image="https://cdn.hashnode.com/res/hashnode/image/upload/v1740080977439/7ad5c157-3c13-4f22-8e83-6d159b135c28.png">
  *Ubuntu 22.04+ required.*

  ***

  Run these commands **in order** to install and properly set up the Pieces Desktop App and it’s core dependencies:

  1. `sudo snap install pieces-os`

  2. `sudo snap connect pieces-os:process-control :process-control`

  3. `sudo snap install pieces-for-developers`

  Then, type `pieces-for-developers` to launch the application directly from your terminal.
</Card>

Your Linux device must be running a supported distribution of Ubuntu—**Ubuntu 22+.**

Click here for documentation [on determining your OS version.](/products/meet-pieces/troubleshooting/linux#checking-ubuntu-version)

## Installation Method

Installation of PiecesOS and the Pieces Desktop App on supported Linux systems is done using the terminal (CLI).

## Post-Installation Tips

Read the documentation below for tips and information to ensure you’re up and running with the latest versions of PiecesOS and the Pieces Desktop App, as well as steps to uninstall Pieces software from your Linux device.

### Updating

The Pieces Desktop App automatically downloads and installs new updates.

You can also manually check for updates to PiecesOS and the Pieces Desktop App by clicking the profile icon nested in the search bar at the top of your Pieces Desktop App view, then selecting `Check for Desktop App Updates` or `Check for PiecesOS Updates.`

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/checking_pieces_desktop_app_for_pieces_os_updates.gif" alt="" align="center" fullwidth="true" />

## Uninstalling

You can uninstall PiecesOS and the Pieces Desktop App using `snap` commands directly from your terminal.

<Callout type="info">
  When running both of these commands, you will be prompted to enter your device’s local account password due to the `sudo` command.
</Callout>

<Steps>
  <Step title="Removing the Pieces Desktop Application">
    `sudo apt remove pieces-for-developers`
  </Step>

  <Step title="Removing PiecesOS">
    `sudo apt remove pieces-os`
  </Step>

  <Step title="Removing Unused Dependencies (Optional)">
    `sudo apt autoremove`
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/uninstall_pfd_from_terminal.png" alt="" align="center" fullwidth="true" />

## Additional Resources

Click here for additional [documentation on troubleshooting](/products/meet-pieces/troubleshooting/linux) or reach out to [support.](/products/support)
