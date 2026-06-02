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
  We're **SOC 2 Type II** certified and never use your data to train models. You can delete everything at any time by removing the `com.pieces.os` and `com.pieces.pfd` folders from your Library (macOS) or equivalent paths on other platforms.
</Callout>

## Where Your Database Lives

| **Platform** | **Default path** |
| --- | --- |
| *macOS* | `/Users/<username>/Library/com.pieces.os/` |
| *Windows (PiecesOS)* | `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\` |
| *Windows (Desktop App)* | `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces for Developers\com.pieces.pfd\` |
| *Linux* | `/home/<username>/.local/share/com.pieces.os/` |

Inside `com.pieces.os`, the `production` folder contains your LTM-2.7 context and all other Pieces data. You can **copy**, **compress**, or **relocate** this folder to sync via OneDrive or migrate to another machine.

The Pieces Desktop App stores additional data in a separate `com.pieces.pfd` folder (`~/Library/com.pieces.pfd/` on macOS, or `...\Pieces for Developers\com.pieces.pfd\` on Windows). For a full backup, copy both folders from their respective parent directories on Windows.

<Callout type="tip">
  Replace `<username>` with your OS account name.
</Callout>

## Finding Your Logs

When opening a GitHub issue or contacting support, attaching recent logs helps diagnose problems quickly.

| **Platform** | **Log path** |
| --- | --- |
| *macOS (PiecesOS)* | `/Users/<username>/Library/com.pieces.os/production/Support/logs/` |
| *macOS (Desktop App)* | `/Users/<username>/Library/com.pieces.pfd/production/logs/` |
| *Windows (PiecesOS)* | `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces OS\com.pieces.os\production\Support\` |
| *Windows (Desktop App)* | `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\Pieces for Developers\com.pieces.pfd\production\logs\` |
| *Linux* | `/home/<username>/.local/share/com.pieces.os/logs/` |

<Callout type="tip">
  On Windows, if `AppData` is hidden in File Explorer, enable `View` → `Show` → `Hidden items`. You can also press `Win+R` and paste the path above. PiecesOS and the Desktop App use different parent folders under `Mesh Intelligent Technologies, Inc\`.
</Callout>

Zip the latest two or three log files from the path above and attach them to your <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> or Discord DM.

## Backup & Restore

Pieces supports two backup approaches. Use **manual folder backup** for a full copy of your on-device database (including Long-Term Memory). Use **Personal Cloud backup** for snapshots of app data you can restore from the Desktop App on any device where you're signed in.

| Method | Best for | Requires |
| --- | --- | --- |
| **Manual folder backup** | Full LTM database, migration, offline archives | Quitting Pieces, copying `com.pieces.os` (and `com.pieces.pfd`) |
| **Personal Cloud backup** | Snippets, Drive files, settings, chat history | Connected [Personal Cloud](/products/desktop/configuration/account#personal-cloud) |

### Manual Backup

Copy your on-device database folders directly. This is the most complete option if you need everything in `production`, including Long-Term Memory context.

<Steps>
  <Step title="Quit all Pieces apps">
    Close the Pieces Desktop App and PiecesOS.
  </Step>

  <Step title="Copy the database folder">
    Copy the entire `com.pieces.os` folder to your backup location (USB, NAS, or cloud storage):

    * **macOS:** `/Users/<username>/Library/` (copy both `com.pieces.os` and `com.pieces.pfd`)
    * **Windows:** Copy `...\Pieces OS\com.pieces.os\` and `...\Pieces for Developers\com.pieces.pfd\` from `C:\Users\<username>\AppData\Local\Mesh Intelligent Technologies, Inc\`
    * **Linux:** `/home/<username>/.local/share/com.pieces.os/`
  </Step>
</Steps>

### Backup via Personal Cloud

Create a snapshot from the Pieces Desktop App. Backups are stored in your personal Pieces Cloud and can be restored or deleted from the same modal.

<Steps>
  <Step title="Open Account Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Account`.
  </Step>

  <Step title="Open Backup & Restore Data">
    Scroll to the *Personal Cloud* section. In *Backup & Restore Data*, click the `Restore Icon` (circular arrow) to open the modal.
  </Step>

  <Step title="Create Backup">
    In the *Create Backup* section, click the `Cloud Icon with Upward Arrow` to upload a new backup to your personal Pieces Cloud.
  </Step>
</Steps>

Cloud backups include snippets, Pieces Drive files, user preferences, Conversational Search data, search and tagging data, and linked account connections (without passwords). They do not replace a full manual copy of your `com.pieces.os` database if you need to preserve raw Long-Term Memory data.

<Callout type="info">
  For the full backup workflow, including what's included, viewing backups, and deleting old snapshots, see [Backup & Restore Data](/products/desktop/configuration/account#backup--restore-data) in Account settings.
</Callout>

## Restore on a New Machine

### Restore a Manual Backup

Use this when you copied `com.pieces.os` (and optionally `com.pieces.pfd`) to another drive or machine.

<Steps>
  <Step title="Install PiecesOS">
    Install PiecesOS on the new machine via the [Pieces Desktop App](/products/desktop/onboarding) or [manual installation](/products/core-dependencies/pieces-os/manual-installation).
  </Step>

  <Step title="Replace the database folder">
    Replace the newly created `com.pieces.os` folder with your backup. Also restore `com.pieces.pfd` if you backed it up.
  </Step>

  <Step title="Restart Pieces">
    Relaunch PiecesOS and the Pieces Desktop App.
  </Step>
</Steps>

### Restore a Personal Cloud Backup

Use this when you created a backup through *Backup & Restore Data* in Account settings.

<Steps>
  <Step title="Connect Personal Cloud">
    On the target machine, open `Settings` → `Account`, scroll to *Personal Cloud*, and connect your cloud if you are not already signed in.
  </Step>

  <Step title="Open Backup & Restore Data">
    In the *Personal Cloud* section, click the `Restore Icon` in *Backup & Restore Data* to open the modal.
  </Step>

  <Step title="Select and Restore">
    In the *Backups* list, find the snapshot you want, then click the `Restore Icon` on that entry and confirm when prompted.
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

## Next Steps

* [Long-Term Memory settings](/products/desktop/configuration/long-term-memory) — clear stored data, app access, and permissions.
* [Account settings](/products/desktop/configuration/account#backup--restore-data) — Personal Cloud backup and restore.
* [Support](/products/support) — report issues and find platform log paths.

## Need Help?

Open a GitHub issue for PiecesOS, the Pieces Desktop App, or any MCP integration at <a target="_blank" href="https://github.com/pieces-app/support/issues">our GitHub repository</a>.

You can also <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support">leave feedback or report a bug here.</a>
