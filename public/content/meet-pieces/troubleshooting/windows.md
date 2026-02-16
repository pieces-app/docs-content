---
title: Issues | Windows
path: /meet-pieces/troubleshooting/windows
visibility: PUBLIC
status: PUBLISHED
description: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected on your Windows issues.
metaTitle: Issues | Windows
metaDescription: Learn about what troubleshooting steps to take if PiecesOS or the Pieces Desktop App isn’t working as expected on your Windows issues.
ogImage: "https://storage.googleapis.com/hashnode_product_documentation_assets/og_images/meet_pieces/meet_pieces_troubleshooting_windows.png"
---

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/troubleshooting_windows.png" alt="Displaying windows.png" align="left" fullwidth="true" />

***

## Installation & Updating Fixes

PiecesOS and the Pieces Desktop App can be downloaded in several ways, and the update process varies based on the method you used, like whether you installed them via WinGet or `.exe` files.

<on-device-storage />

## Manual Installation Methods

If you’re experiencing difficulties with installing PiecesOS or the Pieces Desktop App, you can install both applications manually by downloading the standalone `.exe` or `.appinstaller` files.

### via EXE Files

You can download the individual `.exe` files for PiecesOS and the Pieces Desktop App by clicking the download links below.

<CardGroup cols={2}>
  <Card title="Download — PiecesOS (.EXE)" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/os_server/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE">
    **Step 1:** Download PiecesOS (.EXE)

    *Required Core Dependency*

    Windows 10 (1809) or higher required.
  </Card>

  <Card title="Download — Pieces Desktop App" image="/assets/icons/platform_logos/windows_logo.png" href="https://builds.pieces.app/stages/production/pieces_for_x/windows-exe/download?download=true&product=DOCUMENTATION_WEBSITE">
    **Step 2:** Download Pieces (.EXE)

    *Alternative Method*

    Windows 10 (1809) or higher required.
  </Card>
</CardGroup>

### via WinGet

To install the Pieces Desktop App and PiecesOS using WinGet, follow these steps:

1. **Open a Terminal:** Launch Windows Terminal, Command Prompt, or PowerShell as *administrator*.

2. **Run the WinGet Command:** In the terminal, type `winget install “Pieces”` and press `enter`.

You may be prompted to enter `Y` or `N` to agree or disagree with the terms of use when installing the Pieces Desktop App—type and enter `Y` to proceed with the installation.

3. **Install PiecesOS:** Next, install PiecesOS by typing `winget install “Pieces OS”` and pressing `enter`.

You will be prompted to agree or disagree to the terms of use a second time, so enter `Y` to proceed with the installation.

Once this is finished, you can now launch the Pieces Desktop App by pressing the **Windows symbol** (`⊞`) or toggling the search bar and typing **Pieces,** clicking `Pieces Desktop`.

## Versions & Updates

Many issues can stem from out-of-date plugins, extensions, the desktop app, or PiecesOS itself.

### Updating PiecesOS

<Steps>
  <Step title="Locate the Pieces Icon">
    Find the Pieces Icon (`P`) in your taskbar.
  </Step>
  <Step title="Check for Updates">
    Click the icon to view your update status.
  </Step>
  <Step title="Install Update">
    If an update is available, follow the on-screen prompt to download and install it.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_pieces_os_for_updates.gif" alt="" align="center" fullwidth="true" />

For standalone .EXE installations, updates are checked daily or upon application launch, prompting you to install or delay as needed.

### Updating the Pieces Desktop App

Updating the Pieces Desktop App on Windows can be done directly from the app:

<Steps>
  <Step title="Open the Pieces Desktop App">
    Press the `Windows Icon` and search for Pieces Desktop, open it.
  </Step>

  <Step title="Click Your Username">
    Click your username in the top left of the app.
  </Step>

  <Step title="Hover Over Update">
    Hover over `Update` in the dropdown menu.
  </Step>

  <Step title="Select Component to Update">
    Click on either `Desktop App` or `PiecesOS` from the Update submenu to check for and install updates for that component.
  </Step>

  <Step title="Restart App">
    Restart the app when the update completes.

    <Callout type="info">
      You may also see an update notification automatically when you open either of the apps.
    </Callout>
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_check_pfd_for_updates.gif" alt="" align="center" fullwidth="true" />

## Issues Launching PiecesOS

Some users who have enabled Controlled Folder Access (CFA) as a security measure may receive a notification that Pieces is attempting to bypass this security wall.

To work around this issue, you will need to *add the executable path for PiecesOS* to your allowlist.

<Callout type="alert">
  The reason PiecesOS fails to launch when CFA is enabled is that the executable path for the PiecesOS application writes data to your Documents folder.

  CFA disables and blocks any request to modify files (in this case, writing & saving data), so PiecesOS is unable to launch itself.
</Callout>

Keep in mind that this path references the specific PiecesOS version, and so will change over time as long as you continue to update the software.

You can also disable CFA as a security measure if you do not require it as part of an enterprise scenario or for any other reason.

To decide which apps PiecesOS has access to, you can [easily enable and disable specific sources from the Long-Term Memory Access Control](/products/core-dependencies/pieces-os/quick-menu#long-term-memory-access-control) panel.

## Common Installation Issues

Windows users may encounter installation issues for various reasons, such as out-of-date OS components or incomplete dependencies.

### Checking for Windows Updates

Before installing, ensure your Windows system is fully updated:

1. Click the **Start** button, then select `Settings`

2. Click `Windows Update`

3. Install any pending updates and restart your computer

### Updating the Microsoft Store & App Installer

1. Open the **Microsoft Store**

2. Click on `Library` to check for available updates

3. Update the Microsoft Store and the App Installer if prompted

4. Retry installing the Pieces Suite

## Accessing Pieces Logs

On Windows machines, Pieces writes its log files under your local AppData folder. You'll find two separate folders depending on which component you're using:

* **Pieces OS (POS) logs**:

```plaintext
C:\Users\<USERNAME>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\Support
```

- **Pieces Desktop (PFD) logs**:

```plaintext
C:\Users\<USERNAME>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.pfd\production\Support
```

<Callout type="alert">
  Replace \<USERNAME> with your Windows account name
</Callout>

## Checking Hardware Specifications

It may be necessary to verify your system’s specifications if you experience ongoing issues, especially when attempting to utilize local LLMs.

To check your device specifications on Windows:

* Press the `Windows` key on your keyboard, or the `Windows` icon in the taskbar

* Type `run` and hit `enter`

* Type `dxdiag` and press enter on, or click, the blue `OK` button

The **System** tab displays your processor, the number of CPU cores, and memory (RAM), while the **Display** tab lists your GPU, its manufacturer (NVIDIA, AMD, Intel, etc.), and the available video memory (VRAM).

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_hardware_specs.gif" alt="" align="center" fullwidth="true" />

[Read documentation on the minimum recommended hardware specifications across all OS platforms.](/products/meet-pieces/troubleshooting/cross-platform#hardware-recommendations)

### Checking Windows Version

If the Pieces Installer is not working as intended, you could have an outdated version of Windows. The minimum Windows version that Pieces will run on is **Windows 10 20H0 or higher**.

To check what version of Windows you’re running:

* Press the `Windows` and the `R` keys simultaneously on your keyboard

* A new window will pop up, type `winver` and press `Enter`

A new window will open called **About Windows**, which will display your current Windows version.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/checking_windows_ver.gif" alt="" align="center" fullwidth="true" />

<Callout type="tip">
  If this doesn't work, you're likely using a Windows version older than Windows 10.
</Callout>

## Restart & Retry

If the problem persists, please open a <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> for further assistance or <a target="_blank" href="https://calendar.app.google/WVUDtUfNy5Vst3sH7">book a call with our engineers</a>.