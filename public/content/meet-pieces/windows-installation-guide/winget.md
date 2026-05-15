---
title: WinGet Installation | Windows
path: /meet-pieces/windows-installation-guide/winget
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for Windows using WinGet. A one-command install for developers who prefer package managers.
metaTitle: WinGet Installation | Windows
metaDescription: Install Pieces via WinGet on Windows. One command to install Pieces without leaving your terminal.
---

## WinGet Installation

Install Pieces using WinGet for a streamlined terminal-based setup. WinGet is the Windows Package Manager built into Windows 10 and 11.

### Requirements

* **Windows 10 (1809) or higher** with WinGet installed
* WinGet comes pre-installed on Windows 11 and recent Windows 10 versions

### Install via WinGet

<Steps>
  <Step title="Open Terminal">
    Launch **Windows Terminal**, **Command Prompt**, or **PowerShell**.
  </Step>

  <Step title="Run the install command">
    Copy and run the following command:

    ```bash
    winget install "Pieces"
    ```
  </Step>

  <Step title="Accept the terms">
    When prompted, enter `Y` to agree to the terms of use and proceed with the installation.
  </Step>

  <Step title="Wait for completion">
    WinGet will download and install Pieces. You'll see a success message when complete.
  </Step>
</Steps>

### Updating via WinGet

To update Pieces using WinGet:

```bash
winget upgrade "Pieces"
```

### Uninstalling via WinGet

To remove Pieces using WinGet:

```bash
winget uninstall "Pieces"
```

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [Windows troubleshooting](/products/meet-pieces/troubleshooting/windows) for common solutions.
