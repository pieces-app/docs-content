---
title: Flatpak Installation | Linux
path: /meet-pieces/linux-installation-guide/flatpak
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Linux using Flatpak. A universal package format for Fedora, Arch, Linux Mint, and other distributions.
metaTitle: Install Pieces via Flatpak on Linux | Pieces Docs
metaDescription: Install Pieces via Flatpak on Fedora, Arch, Linux Mint and other distros. Sandboxed installation with manual PiecesOS management.
---

## Flatpak Installation

[Flatpak](https://flatpak.org) is a universal package format that works across most Linux distributions. It's an excellent alternative for users on Fedora, Arch, Linux Mint, Debian, or other distributions that don't include Snap by default. It's also a good choice for users who prefer Flatpak's sandboxing model.

Pieces provides its own Flatpak repository hosted at `builds.pieces.app`, which contains both **PiecesOS** (`com.pieces.os`) and the **Pieces Desktop App** (`com.pieces.pfd`).

### Flatpak Requirements

* **Flatpak:** Install Flatpak using your distro's package manager. Most distributions include it in their repositories. See [flathub.org/setup](https://flathub.org/setup) for distro-specific instructions.
* **Installation scope:** Use `--user` for both packages, or omit it for both. Flatpak does not share runtimes across user and system scopes, so mixing them will fail.
* **User Permissions:** The commands below use `--user`, so no `sudo` is required. Drop `--user` from both install commands if you prefer a system-wide install.

### Install via a software center

Open the PiecesOS `.flatpakref` in GNOME Software, KDE Discover, or another Flatpak-aware software center. That file adds the Pieces repository and the Flathub repository that provides the shared GNOME runtime, then installs PiecesOS.

[Install PiecesOS (`.flatpakref`)](https://builds.pieces.app/pieces-flatpak-repo/com.pieces.os.flatpakref)

After PiecesOS is installed, open the Desktop App `.flatpakref` the same way:

[Install Pieces Desktop App (`.flatpakref`)](https://builds.pieces.app/pieces-flatpak-repo/com.pieces.pfd.flatpakref)

Do not use the older `pieces-flatpak.flatpakrepo` file on its own. A `.flatpakrepo` file only adds a remote and does not declare the runtime source, so the GNOME runtime may be missing.

### Install via Flatpak

Prefer the command line? Run these commands in order.

<Steps>
  <Step title="Install PiecesOS">
    Install PiecesOS, the on-device engine that powers everything — Long-Term Memory, local AI, and MCP.

    ```bash
    flatpak install --user -y --from https://builds.pieces.app/pieces-flatpak-repo/com.pieces.os.flatpakref
    ```

    This adds both the Pieces repository and the Flathub repository that provides the shared GNOME runtime, so no separate setup is needed. It can take a few minutes while Flatpak downloads the runtime. Drop `--user` to install system-wide.
  </Step>

  <Step title="Install Pieces Desktop App">
    Install the Pieces Desktop App, your hub for saving, searching, and managing snippets, screenshots, and developer resources.

    ```bash
    flatpak install --user -y --from https://builds.pieces.app/pieces-flatpak-repo/com.pieces.pfd.flatpakref
    ```

    Use the same scope as the previous command — either `--user` for both, or neither.
  </Step>

  <Step title="Start PiecesOS">
    Start PiecesOS first. It runs as a background service the Desktop App connects to, and the app won't launch it automatically.

    ```bash
    flatpak run com.pieces.os
    ```
  </Step>

  <Step title="Launch the Pieces Desktop App">
    Once PiecesOS is running, launch the Pieces Desktop App. After the first launch, both appear in your application menu.

    ```bash
    flatpak run com.pieces.pfd
    ```

    Always start PiecesOS before the Desktop App.
  </Step>
</Steps>

<Callout type="info">
  Always start PiecesOS first with `flatpak run com.pieces.os`. The Pieces Desktop App does not currently auto-launch PiecesOS when installed via Flatpak. If you launch the Desktop App without PiecesOS running, it will remain on the connection screen until you start PiecesOS manually.
</Callout>

### Updating

Flatpak apps are updated separately from your system packages. You can update Pieces manually or let Flatpak handle it automatically (if your distro supports automatic Flatpak updates).

To manually update both PiecesOS and the Pieces Desktop App, run:

```bash
flatpak update -y com.pieces.os com.pieces.pfd
```

You can also check for updates from the Desktop App by clicking your profile in the top-left corner and selecting `Check for Updates`. Both apps update together.

<Callout type="tip">
  Some desktop environments (like GNOME Software or KDE Discover) can manage Flatpak updates through their graphical interface. Look for Pieces in your software center to update from there.
</Callout>

### Uninstalling

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
  Flatpak stores app data separately from your personal Pieces data. The commands above remove Flatpak-managed state (settings, cache). Your actual Pieces data in `~/.local/share/com.pieces.os/` is preserved and must be deleted manually if desired. See [On-Device Storage](/products/core-dependencies/on-device-storage) for paths on all platforms.
</Callout>

### Troubleshooting

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

**Missing GNOME runtime (`org.gnome.Platform` was not found):**

This happens when Pieces was installed in a different Flatpak scope than Flathub (for example, Flathub as system and Pieces as `--user`). Uninstall both apps, then reinstall from the `.flatpakref` commands above so both remotes are added in the same scope.

```
error: The application com.pieces.os/x86_64/stable requires the runtime org.gnome.Platform/x86_64/48 which was not found
```

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

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [Linux troubleshooting](/products/meet-pieces/troubleshooting/linux) for common solutions.
