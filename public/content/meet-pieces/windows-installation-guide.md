---
title: Installation Guide | Windows
path: /meet-pieces/windows-installation-guide
visibility: PUBLIC
status: PUBLISHED
description: The following guide will help you install and run both PiecesOS and the Pieces for Developers Desktop Application quickly and easily on your Windows device.
metaTitle: Get Started | Windows
metaDescription: Get started with Pieces on Windows – install, configure, troubleshoot and optimize your setup for seamless AI-powered development.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_windows_install.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/trimmed_windows_banner.png" alt="" align="center" fullwidth="true" />

***

## Recommended Installation Method

The recommended installation method on Windows is using the `.appinstaller` file for the Pieces Desktop App.

Download the Pieces Desktop app—after installing Pieces Desktop, PiecesOS will be automatically installed, as it is a necessary dependency.

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/appinstaller/pieces_for_x.appinstaller" gaEvent="doc_download_click" gaPlatform="windows">
    *Recommended Method*

    Windows 10 (1809) or higher required.
  </Card>
</CardGroup>

<Callout type="alert">
  
  PiecesOS is a **required** Core Dependency. When using the recommended <strong>.appinstaller</strong> method, PiecesOS will be installed automatically alongside the Pieces Desktop app—there is no need to download it separately. If you are using an alternative/manual installation method, you may need to download and install PiecesOS manually.

</Callout>

## Install the AppInstaller Files

Now that you have downloaded the `.appinstaller` files, it’s time to install Pieces.

<Steps>
  <Step title="Find Saved Location">
    Open your **Downloads** folder (or wherever you saved the installer) and look for the `.appinstaller` file you just downloaded (e.g., *pieces-appinstaller*).
  </Step>

  <Step title="Open the Installer">
    Double-click the `.appinstaller` file to launch the installation wizard.
  </Step>
</Steps>

Installing via `.appinstaller` or any of the alternative methods, like `.exe`, may cause some user prompt windows to open up—read more about them below.

### System Requirements

Your Windows device must be running **Windows 10 (1809) or higher.**

Click here for a quick guide on [determining your OS version](/products/meet-pieces/troubleshooting/windows#checking-windows-version).

***

| **Component**      | **Minimum**                                                                   | **Recommended**                      | **Notes**                                                        |
| ------------------ | ----------------------------------------------------------------------------- | ------------------------------------ | ---------------------------------------------------------------- |
| *CPU*              | Any modern CPU                                                                | Multi-core CPU                       | Avoid dual-core processors—aim for at least a 4-core CPU.        |
| *RAM (Local Mode)* | 8 GB total system RAM with 2 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running locally.                        |
| *RAM (Cloud Mode)* | 8 GB total system RAM with 1 GB free                                          | 16 GB total system RAM or more       | Applies when PiecesOS is running in cloud mode.                  |
| *Disk Space*       | 2 GB minimum (1 GB for PiecesOS + 0.5–1 GB for data), with at least 4 GB free | 8 GB with at least 6 GB free or more | Ensure additional free space for data storage and future growth. |

***

## Alternative Installations

If you prefer an alternative installation method aside from the `.appinstaller` method, you can also use the `exe` installers or `WinGet` commands through your terminal.

### via EXE

If you cannot use the `.appinstaller` method for any reason, you can also install Pieces via `.exe`.

<CardGroup cols={1}>
  <Card title="Download — Pieces Desktop App (EXE)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/pieces_for_x/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE&_gl=1*1a9yqbf*_gcl_au*OTQ5NDE1NTA4LjE3Mzk0NjU4MzM.*_ga*MTI0OTgzMTMuMTcyNDA5ODQwNg..*_ga_BVYEFRWCYX*MTc0MDc4MjM4Mi44LjAuMTc0MDc4MjM4Mi42MC4wLjA." gaEvent="doc_download_click" gaPlatform="windows">
    *Alternative Method*

    Windows 10 (20H0) or higher required.
  </Card>
</CardGroup>

<Steps>
  <Step title="Find Saved Location">
    Open your **Downloads** folder (or wherever you saved the file) and look for the `.exe` file you just downloaded (e.g., *pieces-exe*).
  </Step>

  <Step title="Open the Installer">
    Double-click the `.exe` file to launch the Windows installation prompt.
  </Step>
</Steps>

### via WinGet

WinGet will allow you to easily install Pieces without having to leave the terminal.

<CardGroup cols={1}>
  <Card title="WinGet — Pieces for Developers" image="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/winget.webp">
    1. Use Windows Terminal, Command Prompt, or PowerShell.

    2. Then, type `winget install “Pieces for Developers”` and press `enter`.

    You will be promoted to agree or disagree to the terms of use a second time, so enter `Y` to proceed with the installation.
  </Card>
</CardGroup>

## On-Screen Prompts

There are a series of on-screen prompts to navigate through when installing the Pieces Desktop App and PiecesOS, through either the `.exe` or `.appinstaller` desktop installation methods.

1. **User Account Control (UAC):** If prompted by Windows’ User Account Control, click `Yes` to allow the installer to make changes.

2. **Install Location:** Choose where to install Pieces (default location is recommended) and click `Install`.

3. **Select Additional Tasks:** Check `Create a desktop shortcut` or `Automatically start Pieces for Developers` if preferred.

4. **Ready to Install:** Click `Install`**.**

5. **Installation Progress & Completion:** Wait for the installation to complete. Once finished, you’ll see a confirmation message. Click `Finish` to close the installer.

## Enterprise & Advanced Security Considerations

Some Windows systems—particularly those in enterprise environments or with advanced security settings—may require using an `.exe` package (default installer) instead of an `.appinstaller` package (AppInstaller) for compatibility reasons.

If you find that your environment is restrictive or that the `.appinstaller` package doesn’t work properly, consider using the `.exe` version or an alternative method.

## Post-Installation Tips

Read the documentation below for some tips and information to make sure you’re up and running with the latest version(s) of PiecesOS and the Pieces Desktop App, as well as steps to uninstall Pieces software from your Windows device.

### Updating

The Pieces Desktop App **automatically downloads and installs new updates.**

You can also manually check for updates to PiecesOS and the Pieces Desktop App by clicking the `Profile` nested in the **Search Bar** at the top of your Pieces Desktop App view, then selecting `Check for Desktop App Updates` or `Check for PiecesOS Updates`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/windows/windows_check_pfd_for_updates.gif" alt="" align="center" fullwidth="true" />

### Uninstalling

Open **Settings,** then find **Apps** and search `Pieces.`

Two applications will appear after you enter the search query—**Pieces Desktop** and **PiecesOS.** Click the three dots to the right of the application title, and click `Uninstall`.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/get_started/windows/uninstalling_on_windows.gif" alt="" align="center" fullwidth="true" />

## Additional Resources

Click here for additional [documentation on troubleshooting](/products/meet-pieces/troubleshooting) or reach out to [support.](/products/support)