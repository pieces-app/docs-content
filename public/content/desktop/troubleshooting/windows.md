---
title: Issues | Windows
path: /desktop/troubleshooting/windows
visibility: PUBLIC
status: PUBLISHED
description: Learn about what troubleshooting steps to take if the Pieces Desktop App isn’t working as expected on your Windows issues.
metaTitle: Troubleshooting Issues on Windows | Pieces Desktop App
metaDescription: Learn about what troubleshooting steps to take if the Pieces Desktop App isn’t working as expected on your Windows device.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/desktop/troubleshooting_windows.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/troubleshooting_windows.png" alt="" align="center" fullwidth="true" />

***

## Installation & Updating Fixes

PiecesOS and the Pieces Desktop App can be downloaded in several ways, and the update process varies based on the method you used, like whether you installed them via WinGet or `.exe` files.

<on-device-storage />

## Manual Installation Methods

If you’re experiencing difficulties installing the Pieces Desktop App, you can install the software manually by downloading the Windows installer or using WinGet.

<CardGroup cols={2}>
  <Card title="Download — Windows" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/os_server/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE" external="true">
    *.EXE*
  </Card>

  <Card title="Download — Windows" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/appinstaller/pieces_for_x.appinstaller?download=true&product=DOCUMENTATION_WEBSITE" external="true">
    *.appinstaller*
  </Card>
</CardGroup>

<Card title="Installing Via WinGet" image="/assets/icons/platform_logos/windows_logo.png">
  You can also install Pieces manually using **WinGet** from your device’s terminal.

  To do so:

  1. Launch Windows Terminal, Command Prompt, or PowerShell as *administrator.*

  2. In the terminal, type `winget install “Pieces”` and press `enter`.

  You may be prompted to enter `Y` or `N` to agree or disagree with the terms of use when installing the Pieces Desktop App—type and enter `Y` to proceed with the installation.
</Card>

## Versions & Updates

Many issues can stem from out-of-date plugins, extensions, or the Desktop App itself.

### Updating the Pieces Desktop App

Updating the Pieces Desktop App on Windows (and macOS) can be done directly within the application:

<Steps>
  <Step title="Open the Pieces Desktop App">
    Press the `Windows Icon` and search for Pieces Desktop, open it
  </Step>

  <Step title="Click Your User Profile">
    Click your `User Profile` in the top left of the main app view
  </Step>

  <Step title="Hover Over Update">
    Hover over `Update` in the dropdown menu that appears
  </Step>

  <Step title="Select Component to Update">
    Click on either `Desktop App` or `PiecesOS` from the Update submenu to check for and install updates for that component
  </Step>

  <Step title="Update Pieces">
    If prompted, click `Download Update` to install available updates.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Troubleshooting/Windows/updating_pieces_desktop.png" alt="" align="center" fullwidth="true" />

You can also select `Check for PiecesOS Updates` from the same menu as an alternative to doing so from the PiecesOS system window in your taskbar.

## Common Installation Issues

Windows users may encounter installation issues for various reasons, such as out-of-date OS components or incomplete dependencies.

### Checking for Windows Updates

Before installing, ensure your Windows system is fully updated:

<Steps>
  <Step title="Open your Settings">
    Click the `Start` button, then select `Settings`.
  </Step>

  <Step title="Find your Updates">
    Click `Windows Update` in the sidebar options.
  </Step>

  <Step title="Install any Updates">
    Install any pending updates and restart your computer.
  </Step>
</Steps>

### Updating the Microsoft Store & App Installer

If you downloaded Pieces software through the Microsoft Store and are experiencing issues with the marketplace interface, try updating the app.

<Steps>
  <Step title="Open the Microsoft Store">
    Press the `Windows` button and search for the **Microsoft Store**, open it.
  </Step>

  <Step title="Find the Library updates">
    Click on `Library `to check for available updates.
  </Step>

  <Step title="Update all recommendations">
    Update the Microsoft Store and the App Installer if prompted.
  </Step>

  <Step title="Reinstall Pieces Suite">
    Now, you can retry installing Pieces Suite.
  </Step>
</Steps>

## Issues Launching PiecesOS

Some users who have enabled Controlled Folder Access (CFA) as a security measure may receive a notification that Pieces is attempting to bypass this security wall.

To work around this issue, you will need to *add the executable path for PiecesOS* to your allowlist.

<Callout type="alert">
  The reason PiecesOS fails to launch when CFA is enabled is that the executable path for the PiecesOS application writes data to your Documents folder.

  CFA disables and blocks any request to modify files (in this case, writing & saving data), so PiecesOS is unable to launch itself.
</Callout>

Keep in mind that this path references the specific PiecesOS version, and so will change over time as long as you continue to update the software. You can also disable CFA as a security measure if you do not require it as part of an enterprise scenario or for any other reason.

PiecesOS uses vision processing to ingest context from foreground applications horizontally.

To decide which apps PiecesOS has access to, you can [easily enable and disable specific sources from the Long-Term Memory Access Control](/products/core-dependencies/pieces-os/quick-menu#long-term-memory-access-control) panel.

## Accessing Pieces Logs

On Windows machines, Pieces writes its log files under your local AppData folder. You’ll find two separate folders depending on which component you’re using:

* **Pieces OS (POS) logs**:\
  `C:\Users\<USERNAME>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\Support`

- **Pieces Desktop (PFD) logs**:\
  `C:\Users\<USERNAME>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.pfd\production\Support`

<Callout type="alert">
  Replace \<USERNAME> with your Windows account name.
</Callout>

## Checking Hardware Specifications

You may need to check your system's specifications if you continue to experience issue[s, especially when trying to use local LLM](/products/core-dependencies/pieces-os/quick-menu#long-term-memory-access-control)s.

To check your device specifications on Windows:

<Steps>
  <Step title="Open the Windows search">
    Press the `Windows` key on your keyboard or the `Windows Icon` in the task bar.
  </Step>

  <Step title="Open Run">
    Type **“run”** and press `enter`.
  </Step>

  <Step title="Find Dxdiag">
    Type `dxdiag` and press `enter` or click the blue `OK` button.
  </Step>
</Steps>

The **System** tab displays your processor, the number of CPU cores, and memory (RAM), while the **Display** tab lists your GPU, its manufacturer (e.g., NVIDIA, AMD, Intel), and the available video memory (VRAM).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_hardware_specs.gif" alt="" align="center" fullwidth="true" />

### Checking Windows Version

If the Pieces Installer isn't working properly, you might be using an outdated version of Windows. Pieces requires at least **Windows 10 20H0 or higher**.

To find out your Windows version, press the `Windows` and `R` keys together, type **winver** in the pop-up window, and press `Enter`.

A new window will open called *About Windows*, which will display your current Windows version.

<Callout type="tip">
  If this doesn't work, you’re likely using a Windows version lower than Windows 10.
</Callout>

### Restart the Pieces Desktop App

After trying any of the fixes above, it’s recommended that you restart your desktop and the Pieces Desktop App.

This ensures all caches are clean and the computer is refreshed.

If the problem persists, please open a <a target="_blank" href="https://github.com/pieces-app/support/issues">**GitHub issue**</a> for further assistance or <a target="_blank" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7">book a call with our engineers</a>.