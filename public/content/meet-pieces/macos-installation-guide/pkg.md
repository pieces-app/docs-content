---
title: PKG Installation | macOS
path: /meet-pieces/macos-installation-guide/pkg
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for macOS using the PKG installer. An alternative method with a guided installation wizard.
metaTitle: PKG Installation | macOS
metaDescription: Install Pieces via PKG on macOS. Download for Apple Silicon or Intel and follow the installation wizard.
---

## PKG Installation

The PKG installer provides a guided installation experience with an installation wizard. Choose the correct version for your Mac's processor.

### Apple Silicon (M-Series / ARM)

<CardGroup cols={1}>
  <Card title="Download — PKG (Apple Silicon)" image="/assets/icons/platform_logos/macos_logo.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd-arm64/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_pkg_arm" gaPlatform="macos">
    *For M1, M2, M3, M4 Macs*

    macOS 13.0 (Ventura) or higher required.
  </Card>
</CardGroup>

### Intel

<CardGroup cols={1}>
  <Card title="Download — PKG (Intel)" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/intel.png" href="https://builds.pieces.app/stages/production/macos_packaging/pkg-pfd/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="macos_pfd_download_pkg_intel" gaPlatform="macos">
    *For pre-2020 Macs*

    macOS 13.0 (Ventura) or higher required.
  </Card>
</CardGroup>

### Install the PKG

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

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [macOS troubleshooting](/products/meet-pieces/troubleshooting/macos) for common solutions.
