---
title: PiecesOS | Troubleshooting
path: /core-dependencies/pieces-os/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: Read about what actionable troubleshooting steps to take if PiecesOS isn’t working as expected on your macOS, Windows, or Linux device.
metaTitle: PiecesOS | Troubleshooting
metaDescription: Read about what actionable troubleshooting steps to take if PiecesOS isn’t working as expected on your macOS, Windows, or Linux device.
---

## Common Installation Issues

Find information on troubleshooting common installation and update issues for PiecesOS.

<on-device-storage />

### Checking System Specifications

Navigate between the grouped tabs below to find information on several common installation issues users experience when downloading and installing PiecesOS.

<Tabs>
  <TabItem title="macOS">
    **macOS | Checking System Specifications**

    It is imperative to install the right version of PiecesOS depending on whether your chip is ARM or Intel-powered.

    Intel and Apple Silicon (ARM) devices run on entirely separate CPU architectures, so downloading the wrong package for your Apple device can cause apps from the Pieces Suite to be rendered useless.

    To determine what CPU architecture your Apple device utilizes:

    1. Click the **Apple () icon** in the top-left corner of your screen.

    2. Select **About This Mac**, and look for the **Overview section.** The first line will contain your CPU type:

    * **Apple Silicon / ARM:** You will see an M-Series processor, e.g., `Apple M3`

    * **Intel:** You will see an Intel processor, e.g., `2.6 GHz Intel Core i7`

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_about_mac.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    **Windows | Checking System Specifications**

    It may be necessary to verify your system’s specifications if you experience ongoing issues, especially when attempting to utilize local LLMs.

    To check your device specifications on Windows:

    * Press the `Windows` key on your keyboard, or the `Windows` icon in the task bar

    * Type `run` and hit `enter`

    * Type `dxdiag` and press enter on, or click, the blue `OK` button

    The **System** tab will display your processor, number of CPU cores, and memory (RAM), while the **Display** tab will list your GPU, it’s maker (NVIDIA, AMD, Intel, etc.) and the available video memory (VRAM).

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_hardware_specs.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    **Linux | Checking System Specifications**

    You can verify your system’s hardware configuration and ensure it meets recommended specifications by running specific commands in your terminal.

    **Checking CPU Information**

    To determine your CPU type and find other important information, type `lscpu` in your terminal and press `Enter`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/lscpu_UBUNTU.png" alt="" align="center" fullwidth="true" />

    **Checking GPU Information**

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/lscpi_UBUNTU.png" alt="" align="center" fullwidth="true" />

    Confirm that your CPU, GPU, and memory resources are sufficient for running PiecesOS and local AI models (if applicable).
  </TabItem>
</Tabs>

<Callout type="tip">
  Once you’ve determined your CPU architecture, [download the correct PiecesOS file accordingly.](/products/core-dependencies/pieces-os/manual-installation#piecesos-download-links)
</Callout>

### Versions & Updates

Many issues can stem from out-of-date plugins, extensions, or PiecesOS itself.

<Tabs>
  <TabItem title="macOS">
    **macOS | Updating PiecesOS**

    To restart and check for updates to PiecesOS on macOS:

    1. Restart PiecesOS

    2. Ensure PiecesOS is running (look for the **Pieces Icon** in your system tray)

    3. Check for and install available updates

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_check_for_updates.png" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    **Windows | Updating PiecesOS**

    To restart and check for updates to PiecesOS on Windows:

    1. Locate the Pieces Icon (`P`) in your taskbar

    2. Click the icon to view your update status

    3. If an update is available, follow the on-screen prompt to download and install it.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_pieces_os_for_updates.gif" alt="" align="center" fullwidth="true" />

    ### Updating PiecesOS (AppInstaller)

    Note that currently, updating PiecesOS if installed via the `.appinstaller` (currently the *Recommended* installation method) files requires that you **quit the Pieces Desktop App**, then proceed with updating PiecesOS.

    If this fails, make sure that the Pieces Desktop App is fully quit, as well as PiecesOS—then relaunch PiecesOS and proceed to download and install the update.
  </TabItem>

  <TabItem title="Linux">
    **Linux | Updating PiecesOS**

    On Linux, PiecesOS and the Pieces Desktop App are distributed via snaps (for Ubuntu-based systems).

    To update PiecesOS on Linux:

    1. Run `snap info pieces-os` to check the current version of PiecesOS

    2. Run `sudo snap refresh` to update PiecesOS if a newer version is available

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/snap_refresh_POS.gif" alt="" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

***

### Checking OS Version

Having an out-of-date operating system version can cause a range of installation issues with PiecesOS, including scenarios in which the entire application refuses to run.

<Tabs>
  <TabItem title="macOS">
    **macOS | Checking OS Version**

    Pieces Suite applications require a minimum macOS version of **macOS Ventura.** If you’re experiencing installation issues, you should check your OS version to ensure it’s up-to-date.

    To determine your Apple device’s version of macOS:

    1. Click the **Apple** icon in the top-left corner of your screen

    2. Select `About This Mac`

    3. Under your device name (i.e., MacBook Air), look for the last line on the list, titled `macOS`

    The `macOS` line will report what version of macOS installed, e.g., `Sequoia 15.1.1`.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_about_mac.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    **Windows | Checking OS Version**

    Windows users may encounter installation issues for various reasons, such as out-of-date OS components or incomplete dependencies.

    Before installing PiecesOS, ensure your Windows system is fully updated:

    1. Click the **Start** button, then select `Settings`

    2. Click `Windows Update`

    3. Install any pending updates and restart your computer

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/checking_windows_ver.gif" alt="" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    **Linux | Checking OS Version**

    If the Pieces Installer is not working as intended, you could have an outdated version of Ubuntu.

    The minimum Ubuntu version that Pieces will run on is **Ubuntu 22.04 and above**.

    To check what version of Ubuntu you’re running:

    * Open **Settings** on Ubuntu

    * Locate the **System** section at the bottom of the left-hand side menu and click it

    * Open the **About** section and locate the **Operating System** label

    This section will will display your Ubuntu version information.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/settings_about_system.gif" alt="" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

***

### Issues Launching PiecesOS (Windows)

Some users who have enabled Controlled Folder Access (CFA) as a security measure may receive a notification that Pieces is attempting to bypass this security wall.

To work around this issue, you must *add the executable path for PiecesOS* to your allowlist.

<Callout type="alert">
  PiecesOS fails to launch when CFA is enabled because the executable path for the application writes data to the Documents folder.

  CFA disables and blocks any request to modify files (in this case, writing & saving data), so PiecesOS cannot launch itself.
</Callout>

Keep in mind that this path references the specific PiecesOS version and will change over time as you continue to update the software.

You can also disable CFA as a security measure if you do not require it as part of an enterprise scenario or for any other reason.

To decide which apps PiecesOS has access to, you can [easily enable and disable specific sources from the Long-Term Memory Access Control](/products/core-dependencies/pieces-os/quick-menu#long-term-memory-access-control) panel.

### Accessing Pieces Logs (Windows)

On Windows machines, Pieces writes its log files under your local AppData folder. You’ll find two separate folders depending on which component you’re using:

* **Pieces OS (POS) logs**:\
  `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\`

- **Pieces Desktop (PFD) logs**:\
  `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces Desktop\com.pieces.os\production\`

<Callout type="alert">
  Replace \<USERNAME> with your Windows account name
</Callout>

## Contact Support

If you’ve ensured your device meets the recommended *and* minimum specifications, you’ve performed a clean installation, updated your OS, and checked PiecesOS for updates, and you’re still experiencing issues, <a target="_blank" href="/products/support">visit our support page for more resources.</a>