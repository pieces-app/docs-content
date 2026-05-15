---
title: EXE Installation | Windows
path: /meet-pieces/windows-installation-guide/exe
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Windows using the EXE installer. A traditional installer for environments where AppInstaller isn't available.
metaTitle: EXE Installation | Windows
metaDescription: Install Pieces via EXE on Windows. A traditional installer with full control over the installation process.
---

## EXE Installation

The EXE installer is an alternative method for installing Pieces on Windows. Use this if the AppInstaller method doesn't work in your environment, such as enterprise systems with restricted policies.

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App (EXE)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/pieces_for_x/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE" gaEvent="windows_pfd_download_exe" gaPlatform="windows">
    *Alternative Method*

    Windows 10 (1809) or higher required.
  </Card>
</CardGroup>

### Install the EXE

<Steps>
  <Step title="Find Saved Location">
    Open your **Downloads** folder (or wherever you saved the file) and look for the `.exe` file you just downloaded.
  </Step>

  <Step title="Open the Installer">
    Double-click the `.exe` file to launch the Windows installation wizard.
  </Step>

  <Step title="User Account Control">
    If prompted by Windows' User Account Control, click `Yes` to allow the installer to make changes.
  </Step>

  <Step title="Choose Install Location">
    Pick a **local** folder (avoid OneDrive or other synced locations). The default path is recommended. Click `Install`.
  </Step>

  <Step title="Select Additional Tasks">
    Optionally check `Create a desktop shortcut` or `Automatically start Pieces` based on your preferences.
  </Step>

  <Step title="Complete Installation">
    Click `Install` and wait for the installation to complete. Click `Finish` when done.
  </Step>
</Steps>

<Callout type="alert">
  **Don't install** Pieces or PiecesOS to **OneDrive** or other **cloud-synced** folders (Dropbox, Google Drive, etc.)—sync can interfere with installs and updates.
</Callout>

### Enterprise Environments

The EXE installer is recommended for enterprise environments or systems with advanced security settings that may block AppInstaller packages.

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [Windows troubleshooting](/products/meet-pieces/troubleshooting/windows) for common solutions.
