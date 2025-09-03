---
title: Troubleshooting
path: /cli/troubleshooting
visibility: PUBLIC
status: PUBLISHED
---

## Having Trouble with Pieces CLI?

If the Pieces CLI isn't working as expected, follow these steps:

### First: Try Updating Pieces CLI

If you're experiencing issues launching the Pieces CLI or using certain commands, the first step is to ensure you have the latest version installed. Outdated versions can cause compatibility issues and unexpected behavior.

**Update your Pieces CLI using your preferred package manager:**

### Update the Package Version(s)

Confirm you're using the latest version of the Pieces CLI using your preferred package manager:

<Callout type="alert">
  **Before updating:** 
  
  - **Windows users:** You may need to run your terminal as administrator for the update to work properly. Right-click on Command Prompt or PowerShell and select "Run as administrator."
  - **All platforms:** Make sure to close any running instances of the Pieces Desktop App and PiecesOS. This prevents conflicts during the update process.
</Callout>

<Tabs>
  <TabItem title="PIP">
    1. To open a terminal on your device, search for `terminal` on macOS/Linux/Windows or `CMD` on Windows, then select the suggested option.

    2. In the newly opened terminal, enter: `pip install pieces-cli -U` to update the Pieces CLI using PIP.
  </TabItem>

  <TabItem title="Conda">
    1. To open a terminal on your device, search for `terminal` on macOS/Linux/Windows or `CMD` on Windows, then select the suggested option.

    2. In the newly opened terminal, enter: `conda update pieces-cli` to update the Pieces CLI using Conda.
  </TabItem>

  <TabItem title="Homebrew">
    1. To open a terminal on your device, search for `terminal` on macOS/Linux/Windows or `CMD` on Windows, then select the suggested option.

    2. In the newly opened terminal, enter: `brew upgrade pieces-cli` to update the Pieces CLI using Homebrew.
  </TabItem>
</Tabs>

An outdated version of PiecesOS might be causing the problems. Be sure to update it, too. 

If not, you can [reinstall it to fix any remaining issues](/products/core-dependencies/pieces-os/manual-installation#manual-download--installation).

## Restart your System After Updates

If you've recently installed or updated PiecesOS or the Pieces CLI, restart your system. This can help apply any system variables that may have been set up during installation.

Contact the [Pieces support team](https://getpieces.typeform.com/to/mCjBSIjF#docs-vscode) if the issue persists.

## Pieces-Specific Fixes

Make sure to check the health and status of PiecesOS. Review the items below if you are having problems with Pieces Drive or Pieces Copilot within the Pieces CLI.

### Check PiecesOS Status

Check to make sure PiecesOS is running.

<pos-check />

*PiecesOS must be running for the Pieces CLI to work.*

### Refreshing Copilot Chats

You may need to restart or refresh the Pieces Copilot chat, especially if you’re using a cloud LLM and disconnect from WiFi.

These scenarios can occasionally cause the LLM to ‘hang’—to appear as if generating a response but eventually timing out, entering an infinite response loop, or experiencing other issues.

To do this, exit the current chat by pressing `⌘+c` (macOS) or `ctrl+c` (Windows/Linux) to force stop the active chat. Then you can re-enter the `ask “query”` command.
