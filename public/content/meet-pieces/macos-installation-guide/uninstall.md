---
title: Complete Uninstall Guide | macOS
path: /meet-pieces/macos-installation-guide/uninstall
visibility: PUBLIC
status: PUBLISHED
description: Completely remove Pieces and all associated data from your Mac. Step-by-step guide to uninstall applications, data folders, preferences, and caches.
metaTitle: Complete Uninstall Guide | macOS
metaDescription: Learn how to completely uninstall Pieces from macOS, including removing all application data, preferences, caches, and saved content.
---

## Complete Uninstall Guide

This guide walks you through completely removing Pieces from your Mac, including all application data, saved snippets, and Long-Term Memory.

<Callout type="warning">
  This process permanently deletes all your saved snippets, conversations, and Long-Term Memory data. If you want to preserve this data, see [backing up your data](/products/privacy-security-your-data#local-backup) before proceeding.
</Callout>

## Complete Uninstall

To remove Pieces and all associated data:

<Steps>
  <Step title="Quit all Pieces processes">
    Click the Pieces icon in your menu bar and select `Quit`. If Pieces isn't responding, open **Activity Monitor** (Applications → Utilities), search for "Pieces", select any Pieces processes, and click the **X** button to force quit.
  </Step>

  <Step title="Remove applications">
    Open **Finder** → **Applications**, then drag both `Pieces` and `PiecesOS` to the Trash.
  </Step>

  <Step title="Remove application data">
    Open **Finder**, press `Cmd + Shift + G` to open "Go to Folder", and navigate to:

    ```
    ~/Library/
    ```

    Delete the following folders if they exist:
    - `com.pieces.os` — Contains your snippets, Long-Term Memory, and engine data
    - `com.pieces.pfd` — Contains Desktop App settings and logs
  </Step>

  <Step title="Remove preferences">
    In the same `~/Library/` location, open the `Preferences` folder and delete any files starting with `com.pieces`:

    ```
    ~/Library/Preferences/com.pieces.*
    ```
  </Step>

  <Step title="Remove caches">
    Navigate to the `Caches` folder and delete any Pieces-related folders:

    ```
    ~/Library/Caches/com.pieces.*
    ```
  </Step>

  <Step title="Empty Trash">
    Right-click the Trash icon in your Dock and select `Empty Trash` to permanently delete the files.
  </Step>
</Steps>

### Homebrew Users

If you installed Pieces via Homebrew, run this command instead of manually removing the applications:

```bash
brew uninstall --cask pieces
```

Then continue with Steps 3-6 above to remove application data.

### Terminal Commands (Advanced)

For users comfortable with Terminal, you can run these commands to remove everything at once:

```bash
# Quit Pieces processes
pkill -f "Pieces" 2>/dev/null
pkill -f "PiecesOS" 2>/dev/null

# Remove applications
rm -rf /Applications/Pieces.app
rm -rf /Applications/PiecesOS.app

# Remove application data
rm -rf ~/Library/com.pieces.os
rm -rf ~/Library/com.pieces.pfd

# Remove preferences
rm -f ~/Library/Preferences/com.pieces.*

# Remove caches
rm -rf ~/Library/Caches/com.pieces.*
```

<Callout type="alert">
  These commands permanently delete files without moving them to Trash. Double-check before running.
</Callout>

## Verify Removal

To confirm Pieces has been completely removed:

1. Open **Spotlight** (Cmd + Space) and search for "Pieces" — no results should appear
2. Open **Finder**, press `Cmd + Shift + G`, and check that `~/Library/com.pieces.os` no longer exists

## Reinstalling

If you want to reinstall Pieces later, see the [macOS installation guide](/products/meet-pieces/macos-installation-guide) for fresh install instructions.
