---
title: Snap Installation | Linux
path: /meet-pieces/linux-installation-guide/snap
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Linux using Snap. The recommended method for Ubuntu users with automatic updates and system integration.
metaTitle: Snap Installation | Linux
metaDescription: Install Pieces via Snap on Ubuntu. One-command install with automatic updates, system interfaces, and easy management.
---

## Snap Installation (Recommended for Ubuntu)

Snap is the recommended installation method for Ubuntu users. It provides automatic updates, system integration, and simple management through terminal commands.

### Snap Requirements

* **Snap Support:** Ensure `snapd` is installed and enabled. Most Ubuntu releases include it by default.
* **Administrator Access:** You'll need `sudo` privileges to install snap packages.
* **Ubuntu 22.04+** or a compatible distribution with Snap support.

### Install via Snap

<Card title="Install via Snap" image="/assets/icons/platform_logos/ubuntu_logo.png">
  *Ubuntu 22.04+ required.*

  ***

  Run these commands **in order** to install and properly set up the Pieces Desktop App and its core dependencies:

  1. `sudo snap install pieces-os`

  2. `sudo snap connect pieces-os:process-control :process-control`

  3. `sudo snap install pieces-for-developers`

  Then, type `pieces-for-developers` to launch the application directly from your terminal.
</Card>

Click here for documentation [on determining your OS version.](/products/meet-pieces/troubleshooting/linux#checking-ubuntu-version)

### Connect System Interfaces

After installing via Snap, run `pieces-os.doctor` in your terminal. The script outputs a command you can copy and paste to connect all interfaces with the system. This step is required for full functionality, including features like [LTM Audio](/products/desktop/configuration/long-term-memory#ltm-audio).

### Updating

The Pieces Desktop App automatically downloads and installs new updates.

You can also manually check for updates by hovering over your username in the top left, then hovering over `Update` and selecting either `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/checking_pieces_desktop_app_for_pieces_os_updates.gif" alt="Checking for PiecesOS updates in the Pieces Desktop App on Linux" align="center" fullwidth="true" />

### Uninstalling

You can uninstall PiecesOS and the Pieces Desktop App using `snap` commands directly from your terminal.

<Callout type="info">
  When running these commands, you will be prompted to enter your device's local account password due to the `sudo` command.
</Callout>

<Steps>
  <Step title="Removing the Pieces Desktop Application">
    `sudo snap remove pieces-for-developers`
  </Step>

  <Step title="Removing PiecesOS">
    `sudo snap remove pieces-os`
  </Step>
</Steps>

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [Linux troubleshooting](/products/meet-pieces/troubleshooting/linux) for common solutions.
