---
title: Homebrew Installation | macOS
path: /meet-pieces/macos-installation-guide/homebrew
visibility: PUBLIC
status: PUBLISHED
description: Install Pieces for macOS using Homebrew. A one-command install for developers who prefer package managers.
metaTitle: Homebrew Installation | macOS
metaDescription: Install Pieces via Homebrew on macOS. One command to install both Pieces Desktop and PiecesOS.
---

## Homebrew Installation

Install Pieces using Homebrew for a streamlined terminal-based setup. This method automatically installs both the Pieces Desktop App and PiecesOS.

### Requirements

* **Homebrew:** Ensure Homebrew is installed on your system. Visit [brew.sh](https://brew.sh) if you need to install it.
* **macOS 13.0 (Ventura) or higher**

### Install via Homebrew

<Steps>
  <Step title="Open Terminal">
    Launch **Terminal** from Applications > Utilities, or use Spotlight (⌘ + Space) and search for "Terminal".
  </Step>

  <Step title="Run the install command">
    Copy and run the following command:

    ```bash
    brew install --cask pieces
    ```
  </Step>

  <Step title="Enter your password">
    If prompted, enter your administrator password to allow the installation.
  </Step>

  <Step title="Wait for completion">
    Homebrew will download and install both the Pieces Desktop App and PiecesOS. You'll see a success message when complete.
  </Step>
</Steps>

### Updating via Homebrew

To update Pieces using Homebrew:

```bash
brew upgrade --cask pieces
```

### Uninstalling via Homebrew

To remove Pieces using Homebrew:

```bash
brew uninstall --cask pieces
```

## Next Steps

After installation, explore [Conversational Search](/products/desktop/conversational-search) to start chatting with your memories, or configure [Long-Term Memory](/products/desktop/configuration/long-term-memory) to customize how Pieces captures your workflow context.

If you encounter issues, see [macOS troubleshooting](/products/meet-pieces/troubleshooting/macos) for common solutions.
