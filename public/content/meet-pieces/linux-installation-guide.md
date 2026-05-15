---
title: Installation Guide | Linux
path: /meet-pieces/linux-installation-guide
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Linux via Snap or Flatpak. Choose the installation method that works best for your distribution.
metaTitle: Get started | Linux
metaDescription: Get started with Pieces on Linux – install via Snap or Flatpak, then configure and optimize your setup for AI-powered development.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_linux_install.png"
---

## Install Pieces for Linux

Pieces for Linux is available via **Snap** (recommended for Ubuntu) or **Flatpak** (for Fedora, Arch, Linux Mint, and other distros). Choose the method that works best for your system.

<InstallMethodGroup>
  <InstallMethodCard title="Snap" href="/products/meet-pieces/linux-installation-guide/snap" recommended={true}>
    Snap package for Ubuntu and Snap-supported distributions.
  </InstallMethodCard>
  <InstallMethodCard title="Flatpak" href="/products/meet-pieces/linux-installation-guide/flatpak">
    Flatpak package for Fedora, Arch, and other distributions.
  </InstallMethodCard>
</InstallMethodGroup>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_linux_install.png" alt="Pieces for Linux installation guide banner" align="center" fullwidth="true" />

### General Requirements

* **Minimum OS:** Ubuntu 22+ or equivalent modern Linux distribution
* **Display Server:** Pieces is primarily **supported** on **X11**. **Wayland** support requires manual steps. Run `pieces-os.doctor` after install (Snap only) and follow its output. If **Long-Term Memory** or screen-related features misbehave, especially in some VMs, try logging in with an **X11 session** or see [Linux troubleshooting](/products/meet-pieces/troubleshooting/linux).

<Callout type="tip">
  Check your session with `echo $XDG_SESSION_TYPE` (`wayland` or `x11`). On **Wayland**, use `pieces-os.doctor` to wire up interfaces; labels in **Settings → System** vary by distro.
</Callout>

## Additional Resources

Click here for additional [documentation on troubleshooting](/products/meet-pieces/troubleshooting/linux) or reach out to [support.](/products/support)
