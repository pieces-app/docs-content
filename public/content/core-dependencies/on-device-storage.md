---
title: On-Device Storage
path: /core-dependencies/on-device-storage
visibility: PUBLIC
status: PUBLISHED
description: Everything you save in Pieces lives locally first. Here's exactly where to find it—and how to back up, restore, or reset your data.
metaTitle: On-Device Storage & Logs | Pieces Docs
metaDescription: Learn where Pieces stores your database and logs on macOS, Windows, and Linux. Backup, restore, or delete data locally with SOC 2-certified security.
---

## Local-First Architecture

Pieces stores and processes everything on your device by default—code snippets, LTM-2.7 memory, user settings, Conversational Search history, and diagnostic logs all stay local.

**When data can move to the cloud:** Only when you explicitly enable **Personal Cloud** or use a cloud-based model provider (OpenAI, Anthropic, Google). In those cases, data is handled by the provider's privacy policy.

<Callout type="tip">
  We're **SOC 2 Type II** certified and never use your data to train models. You can delete everything at any time by removing the `com.pieces.os` folder.
</Callout>

## Where Your Database Lives

| **Platform** | **Default path** |
| --- | --- |
| *macOS* | `/Users/<username>/Library/com.pieces.os/` |
| *Windows* | `C:/Users/<username>/Documents/com.pieces.os/` |
| *Linux* | `/home/<username>/.local/share/com.pieces.os/` |

Inside `com.pieces.os`, the `production` folder contains your LTM-2.7 context and all other Pieces data. You can **copy**, **compress**, or **relocate** this folder to sync via OneDrive or migrate to another machine.

<Callout type="tip">
  Replace `<username>` with your OS account name.
</Callout>

## Finding Your Logs

When opening a GitHub issue or contacting support, attaching recent logs helps diagnose problems quickly.

| **Platform** | **Log path** |
| --- | --- |
| *macOS* | `/Users/<username>/Library/com.pieces.os/production/support/logs/` |
| *Windows* | `C:/Users/<username>/Documents/com.pieces.os/production/support/logs` |
| *Linux* | `/home/<username>/.local/share/com.pieces.os/logs/` |

Logs rotate daily and are timestamped (e.g., `log-05062025`). Zip the latest two or three files and attach them to your <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> or Discord DM.

## Create a Manual Backup

<Steps>
  <Step title="Quit all Pieces apps">
    Close the Pieces Desktop App and PiecesOS.
  </Step>

  <Step title="Copy the database folder">
    Copy the entire `com.pieces.os` folder to your backup location (USB, NAS, or cloud storage):

    * **macOS:** `/Users/<username>/Library/com.pieces.os/`
    * **Windows:** `C:/Users/<username>/Documents/com.pieces.os/`
    * **Linux:** `/home/<username>/.local/share/com.pieces.os/`
  </Step>
</Steps>

## Restore on a New Machine

<Steps>
  <Step title="Install PiecesOS">
    Install PiecesOS on the new machine via the [Pieces Desktop App](/products/desktop/onboarding) or [manual installation](/products/core-dependencies/pieces-os/manual-installation).
  </Step>

  <Step title="Replace the database folder">
    Replace the newly created `com.pieces.os` folder with your backup.
  </Step>

  <Step title="Restart Pieces">
    Relaunch PiecesOS and the Pieces Desktop App.
  </Step>
</Steps>

## Start Fresh (Reset)

<Steps>
  <Step title="Quit Pieces">
    Close the Pieces Desktop App and PiecesOS.
  </Step>

  <Step title="Rename the production folder">
    Rename the `production` folder inside `com.pieces.os` to something else (e.g., `production-backup`).
  </Step>

  <Step title="Relaunch Pieces">
    Relaunch PiecesOS. It will create a brand-new, empty database. Keep the renamed folder as a backup in case you need it.
  </Step>
</Steps>

***

## Need Help?

Open a GitHub issue for PiecesOS, the Pieces Desktop App, or any MCP integration at <a target="_blank" href="https://github.com/pieces-app/support/issues">our GitHub repository</a>.

You can also <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support">leave feedback or report a bug here.</a>
