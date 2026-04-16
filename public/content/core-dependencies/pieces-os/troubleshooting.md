---
title: Troubleshooting PiecesOS
path: /core-dependencies/pieces-os/troubleshooting
visibility: PUBLIC
status: PUBLISHED
description: Fix common PiecesOS installation issues, check system specs, update PiecesOS, and find logs on macOS, Windows, and Linux.
metaTitle: Troubleshooting PiecesOS | Pieces Docs
metaDescription: Fix common PiecesOS installation issues, check system specs, update PiecesOS, and find logs on macOS, Windows, and Linux.
---

<on-device-storage />

## Installation Issues

### Cloud-Synced Folders

If you installed PiecesOS to **OneDrive**, **iCloud Drive**, or another synced folder, you may see install failures, crashes, or broken updates. **Uninstall**, then **reinstall** to the **default path** on a local drive. See [Manual Installation](/products/core-dependencies/pieces-os/manual-installation).

### Checking System Specifications

<Tabs>
  <TabItem title="macOS">
    Install the correct PiecesOS build for your chip (ARM vs Intel):

    <Steps>
      <Step title="Open About This Mac">
        Click the **Apple () icon** in the top-left corner and select **About This Mac**.
      </Step>

      <Step title="Identify your processor">
        Look for your processor type:

        * **Apple Silicon:** M-series (e.g., `Apple M3`)
        * **Intel:** Intel processor (e.g., `2.6 GHz Intel Core i7`)
      </Step>
    </Steps>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_about_mac.gif" alt="Checking macOS CPU architecture via About This Mac" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    Check your device specs if you're experiencing issues, especially with local LLMs:

    <Steps>
      <Step title="Open the Run dialog">
        Press the `Windows` key, type `run`, and press Enter.
      </Step>

      <Step title="Launch DirectX Diagnostic">
        Type `dxdiag` and press Enter.
      </Step>

      <Step title="Review your specs">
        The **System** tab shows CPU and RAM; the **Display** tab shows GPU and VRAM.
      </Step>
    </Steps>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_hardware_specs.gif" alt="Checking Windows hardware specs using dxdiag" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    Verify your hardware meets requirements:

    * **CPU:** Run `lscpu` in your terminal
    * **GPU:** Run `lspci | grep -i vga` in your terminal

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/lscpu_UBUNTU.png" alt="Terminal output of lscpu command on Ubuntu" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

<Callout type="tip">
  Once you've determined your CPU architecture, [download the correct PiecesOS build.](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation)
</Callout>

## Updating PiecesOS

Many issues stem from running an outdated version. Check for updates from the [Quick Menu](/products/core-dependencies/pieces-os/quick-menu#checking-for-updates) or follow the platform-specific steps below.

<Tabs>
  <TabItem title="macOS">
    <Steps>
      <Step title="Find the Pieces icon">
        Look for the **Pieces icon** in your menu bar.
      </Step>

      <Step title="Open the Quick Menu">
        Click the icon to open the Quick Menu.
      </Step>

      <Step title="Install the update">
        If an update is available, click to install it.
      </Step>
    </Steps>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/core_desktop_meet-pieces_orgs_paid-plans_12.3.6/core-dependencies/quick-menu_check_for_updates.png" alt="Checking for PiecesOS updates via Quick Menu on macOS" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    <Steps>
      <Step title="Open the Quick Menu">
        Click the **Pieces icon** in your taskbar.
      </Step>

      <Step title="Check your update status">
        The Quick Menu displays your current version and whether an update is available.
      </Step>

      <Step title="Install the update">
        Follow the on-screen prompt if an update is available.
      </Step>
    </Steps>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/windows_checking_pieces_os_for_updates.gif" alt="Checking PiecesOS for updates on Windows taskbar" align="center" fullwidth="true" />

    <Callout type="info">
      If installed via `.appinstaller`, quit the Pieces Desktop App before updating PiecesOS. If the update fails, quit both apps completely, then relaunch PiecesOS.
    </Callout>
  </TabItem>

  <TabItem title="Linux">
    <Steps>
      <Step title="Check your current version">
        Run `snap info pieces-os` in your terminal.
      </Step>

      <Step title="Update PiecesOS">
        Run `sudo snap refresh` to install the latest version.
      </Step>
    </Steps>

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/snap_refresh_POS.gif" alt="Running snap refresh to update PiecesOS on Linux" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

## Checking OS Version

An outdated operating system can prevent PiecesOS from running. Minimum requirements:

| **macOS** | **Windows** | **Linux** |
| --- | --- | --- |
| macOS 12.0 (Monterey)+ | Windows 10 (v.1809)+ | Ubuntu 22+ |

<Tabs>
  <TabItem title="macOS">
    Click **Apple () icon** > **About This Mac** — the `macOS` line shows your version (e.g., `Sequoia 15.1.1`).

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/macos/macos_checking_about_mac.gif" alt="Checking macOS version via About This Mac" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Windows">
    Go to **Settings** > **Windows Update** and install any pending updates.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/windows/checking_windows_ver.gif" alt="Checking Windows version using winver command" align="center" fullwidth="true" />
  </TabItem>

  <TabItem title="Linux">
    Open **Settings** > **System** > **About** to find your Ubuntu version. Minimum: **Ubuntu 22.04**.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/meet_pieces_assets/meet_pieces/troubleshooting/linux/settings_about_system.gif" alt="Checking Ubuntu version in System Settings" align="center" fullwidth="true" />
  </TabItem>
</Tabs>

## Windows: Controlled Folder Access

If you've enabled Controlled Folder Access (CFA), PiecesOS may fail to launch because it writes data to the Documents folder. Add the PiecesOS executable path to your CFA allowlist, or disable CFA if it's not required.

## Finding Pieces Logs

Attach recent logs when opening a GitHub issue or contacting support—it helps diagnose problems in minutes.

**PiecesOS logs:**

| **Platform** | **Path** |
| --- | --- |
| *macOS* | `/Users/<username>/Library/com.pieces.os/production/support/logs/` |
| *Windows* | `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\` |
| *Linux* | `/home/<username>/.local/share/com.pieces.os/logs/` |

**Pieces Desktop logs (Windows):**
```
C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces Desktop\com.pieces.os\production\
```

<Callout type="tip">
  Replace `<username>` with your OS account name. Zip the latest two or three log files and attach them to your <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a>.
</Callout>

***

If you've tried everything above and still have issues, <a target="_blank" href="/products/support">visit our support page</a> for additional resources.
