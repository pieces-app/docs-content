---
title: AppInstaller | Windows
path: /meet-pieces/windows-installation-guide/appinstaller
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Windows using the AppInstaller. The recommended method with automatic PiecesOS installation.
metaTitle: AppInstaller | Windows
metaDescription: Install Pieces via AppInstaller on Windows. The recommended method that automatically installs PiecesOS alongside the Desktop App.
---

## AppInstaller (Recommended)

The AppInstaller method is the recommended way to install Pieces on Windows. It automatically installs PiecesOS alongside the Pieces Desktop App.

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/appinstaller/pieces_for_x.appinstaller" gaEvent="windows_pfd_download_appinstaller" gaPlatform="windows">
    *Recommended Method*

    Windows 10 (1809) or higher required.
  </Card>
</CardGroup>

<Callout type="alert">
  PiecesOS is a **required** Core Dependency. When using the AppInstaller method, PiecesOS will be installed automatically alongside the Pieces Desktop App—there is no need to download it separately.
</Callout>

### Install the AppInstaller

<Steps>
  <Step title="Find Saved Location">
    Open your **Downloads** folder (or wherever you saved the installer) and look for the `.appinstaller` file you just downloaded.
  </Step>

  <Step title="Open the Installer">
    Double-click the `.appinstaller` file to launch the installation wizard.
  </Step>

  <Step title="Follow the prompts">
    If prompted by Windows' User Account Control, click `Yes` to allow the installer to make changes.
  </Step>
</Steps>

### System Requirements

| **Component**      | **Minimum**                                                                   | **Recommended**                      | **Notes**                                                        |
| ------------------ | ----------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------- |
| *OS Version*       | Windows 10 (1809)                                                             | Windows 11                           | 64-bit required.                                                 |
| *CPU*              | Any modern CPU                                                                | Multi-core CPU                       | Avoid dual-core processors—aim for at least a 4-core CPU.        |
| *RAM (Local Mode)* | 8 GB total system RAM with 2 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running locally.                        |
| *RAM (Cloud Mode)* | 8 GB total system RAM with 1 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running in cloud mode.                  |
| *Disk Space*       | 2 GB minimum (1 GB for PiecesOS + 0.5–1 GB for data), with at least 4 GB free | 8 GB with at least 6 GB free or more | Ensure additional free space for data storage and future growth. |

Click here for a quick guide on [determining your OS version](/products/meet-pieces/troubleshooting/windows#checking-windows-version).

<Callout type="alert">
  **Don't install** Pieces or PiecesOS to **OneDrive** or other **cloud-synced** folders (Dropbox, Google Drive, etc.)—sync can interfere with installs and updates. Use the **default path** on a local drive.
</Callout>

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [Windows troubleshooting](/products/meet-pieces/troubleshooting/windows) for common solutions.
