---
title: Installation Guide | Linux
path: /meet-pieces/linux-installation-guide
visibility: PUBLIC
status: PUBLISHED
description: The following guide will help you install and run both PiecesOS and the Pieces Desktop Application quickly and easily on your Linux device.
metaTitle: Get started | Linux
metaDescription: Get started with Pieces on Linux – install, configure, troubleshoot and optimize your setup for seamless AI-powered development.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_linux_install.png"
---

<install-guide-buttons />

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_linux_install.png" alt="Pieces for Linux installation guide banner" align="center" fullwidth="true" />

***

## Install Pieces for Linux

Pieces for Linux is available via **Snap** (recommended for Ubuntu) or **Flatpak** (for Fedora, Arch, Linux Mint, and other distros). Choose the method that works best for your system.

### General Requirements

* **Minimum OS:** Ubuntu 22+ or equivalent modern Linux distribution
* **Display Server:** Pieces is primarily **supported** on **X11**. **Wayland** support requires manual steps. Run `pieces-os.doctor` after install (Snap only) and follow its output. If **Long-Term Memory** or screen-related features misbehave, especially in some VMs, try logging in with an **X11 session** or see [Linux troubleshooting](/products/meet-pieces/troubleshooting/linux).

<Callout type="tip">
  Check your session with `echo $XDG_SESSION_TYPE` (`wayland` or `x11`). On **Wayland**, use `pieces-os.doctor` to wire up interfaces; labels in **Settings → System** vary by distro.
</Callout>

## Snap Installation (Recommended for Ubuntu)

Snap is the recommended installation method for Ubuntu users.

### Snap Requirements

* **Snap Support:** Ensure `snapd` is installed and enabled. Most Ubuntu releases include it by default.
* **Administrator Access:** You'll need `sudo` privileges to install snap packages.

<Card title="Install via Snap" image="/assets/icons/platform_logos/ubuntu_logo.png">
  *Ubuntu 22.04+ required.*

  ***

  Run these commands **in order** to install and properly set up the Pieces Desktop App and its core dependencies:

  1. `sudo snap install pieces-os`

  2. `sudo snap connect pieces-os:process-control :process-control`

  3. `sudo snap install pieces-for-developers`
  
  Run `pieces-os.doctor`. The script outputs a command; copy and paste it into your terminal to connect all interfaces with the system.

  Then, type `pieces-for-developers` to launch the application directly from your terminal.
</Card>

Click here for documentation [on determining your OS version.](/products/meet-pieces/troubleshooting/linux#checking-ubuntu-version)

### Connect System Interfaces (Snap)

After installing via Snap, run `pieces-os.doctor` in your terminal. The script outputs a command you can copy and paste to connect all interfaces with the system. This step is required for full functionality, including features like [LTM Audio](/products/desktop/configuration/long-term-memory#ltm-audio).

### Updating (Snap)

The Pieces Desktop App automatically downloads and installs new updates.

You can also manually check for updates by hovering over your username in the top left, then hovering over `Update` and selecting either `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started_linux/checking_pieces_desktop_app_for_pieces_os_updates.gif" alt="Checking for PiecesOS updates in the Pieces Desktop App on Linux" align="center" fullwidth="true" />

### Uninstalling (Snap)

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

***

## Flatpak Installation (Alternative)

[Flatpak](https://flatpak.org) is a universal package format that works across most Linux distributions. It's an excellent alternative for users on Fedora, Arch, Linux Mint, Debian, or other distributions that don't include Snap by default. It's also a good choice for users who prefer Flatpak's sandboxing model.

Pieces provides its own Flatpak repository hosted at `builds.pieces.app`, which contains both **PiecesOS** (`com.pieces.os`) and the **Pieces Desktop App** (`com.pieces.pfd`).

### Flatpak Requirements

* **Flatpak Runtime:** Install Flatpak using your distro's package manager. Most distributions include it in their repositories. See [flathub.org/setup](https://flathub.org/setup) for distro-specific instructions.
* **Flathub Repository:** The Flathub repository provides shared runtime dependencies that Pieces requires. It must be added before installing Pieces.
* **User Permissions:** The Pieces repository is added with the `--user` flag, so no `sudo` is required for installation.

### Install via Flatpak

Follow these steps in order to install Pieces via Flatpak. All commands are run in your terminal.

<Steps>
  <Step title="Add Flathub Repository">
    Flathub provides shared runtime dependencies that Pieces requires. If you haven't already added Flathub to your system, run:

    ```bash
    flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
    ```

    This command is safe to run even if Flathub is already configured. It will skip if the repository already exists.
  </Step>

  <Step title="Add the Pieces Flatpak Repository">
    Add the official Pieces Flatpak repository to your system. This repository hosts both PiecesOS and the Pieces Desktop App:

    ```bash
    flatpak remote-add --user --if-not-exists --from pieces-flatpak https://builds.pieces.app/pieces-flatpak-repo/pieces-flatpak.flatpakrepo
    ```

    The `--user` flag installs the repository for your user account only, so no `sudo` is required.
  </Step>

  <Step title="Install PiecesOS">
    Install PiecesOS, the local engine that powers all Pieces functionality. PiecesOS runs on-device for speed, privacy, and offline use:

    ```bash
    flatpak install -y pieces-flatpak com.pieces.os
    ```

    This may take a few minutes as Flatpak downloads the required runtime dependencies.
  </Step>

  <Step title="Install Pieces Desktop App">
    Install the Pieces Desktop App, your hub for saving, searching, and managing code snippets, screenshots, and developer resources:

    ```bash
    flatpak install -y pieces-flatpak com.pieces.pfd
    ```
  </Step>

  <Step title="Launch Pieces">
    **Important:** You must start PiecesOS first. It runs as a background service that the Desktop App connects to. The Desktop App will not launch PiecesOS automatically.

    ```bash
    flatpak run com.pieces.os
    ```

    Once PiecesOS is running, launch the Pieces Desktop App:

    ```bash
    flatpak run com.pieces.pfd
    ```

    After the first launch, both apps will appear in your application menu. Always launch PiecesOS before the Desktop App.
  </Step>
</Steps>

<Callout type="info">
  Always start PiecesOS first with `flatpak run com.pieces.os`. The Pieces Desktop App does not currently auto-launch PiecesOS when installed via Flatpak. If you launch the Desktop App without PiecesOS running, it will remain on the connection screen until you start PiecesOS manually.
</Callout>

### Updating (Flatpak)

Flatpak apps are updated separately from your system packages. You can update Pieces manually or let Flatpak handle it automatically (if your distro supports automatic Flatpak updates).

To manually update both PiecesOS and the Pieces Desktop App, run:

```bash
flatpak update -y com.pieces.os com.pieces.pfd
```

You can also check for updates within the Pieces Desktop App by hovering over your username in the top left, then hovering over `Update` and selecting `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

<Callout type="tip">
  Some desktop environments (like GNOME Software or KDE Discover) can manage Flatpak updates through their graphical interface. Look for Pieces in your software center to update from there.
</Callout>

### Uninstalling (Flatpak)

You can remove PiecesOS and the Pieces Desktop App using Flatpak commands. The process involves stopping any running instances, removing the apps, and optionally removing the Pieces repository.

<Steps>
  <Step title="Stop Running Instances">
    Before uninstalling, stop any running Pieces processes:

    ```bash
    flatpak kill com.pieces.pfd || true
    flatpak kill com.pieces.os || true
    ```
  </Step>

  <Step title="Remove the Pieces Desktop App">
    Uninstall the Pieces Desktop App and its Flatpak-managed data:

    ```bash
    flatpak uninstall -y --delete-data com.pieces.pfd
    ```
  </Step>

  <Step title="Remove PiecesOS">
    Uninstall PiecesOS and its Flatpak-managed data:

    ```bash
    flatpak uninstall -y --delete-data com.pieces.os
    ```
  </Step>

  <Step title="Remove the Pieces Repository (Optional)">
    If you no longer want to receive updates from the Pieces Flatpak repository, remove it:

    ```bash
    flatpak remote-delete --user pieces-flatpak
    ```
  </Step>

  <Step title="Clean Up Unused Runtimes (Optional)">
    Remove any shared runtimes that are no longer needed by other Flatpak apps:

    ```bash
    flatpak uninstall -y --unused
    ```
  </Step>
</Steps>

<Callout type="info">
  Flatpak stores app data separately from your personal Pieces data. The commands above remove Flatpak-managed state (settings, cache). Your actual Pieces data in `~/Documents/com.pieces.os` and `~/Documents/com.pieces.pfd` is preserved and must be deleted manually if desired.
</Callout>

### Troubleshooting (Flatpak)

If you encounter issues with the Flatpak installation, try these common solutions.

**Pieces Desktop App can't connect to PiecesOS:**

PiecesOS must be running before you launch the Pieces Desktop App. Check if it's running and start it if needed:

```bash
# Check if PiecesOS is running
flatpak ps | grep pieces

# Start PiecesOS manually if it's not running
flatpak run com.pieces.os
```

**Permission or sandbox issues:**

If features aren't working correctly, reset the Flatpak permissions for both apps:

```bash
flatpak permission-reset com.pieces.os
flatpak permission-reset com.pieces.pfd
```

Then restart both applications.

**Verify the Pieces repository is accessible:**

If installation fails, confirm the Pieces repository is reachable:

```bash
curl -fsSIL https://builds.pieces.app/pieces-flatpak-repo/summary
```

You should see `HTTP/2 200` after the redirect completes. The `-L` flag follows the redirect to the storage backend.

**Complete reset (keeps personal data):**

If you need a fresh start, uninstall and reinstall:

```bash
flatpak kill com.pieces.pfd || true
flatpak kill com.pieces.os || true
flatpak uninstall -y --delete-data com.pieces.pfd com.pieces.os
```

Then follow the installation steps above to reinstall.

***

## Additional Resources

Click here for additional [documentation on troubleshooting](/products/meet-pieces/troubleshooting/linux) or reach out to [support.](/products/support)
