---
title: On-Device Storage
path: /core-dependencies/on-device-storage
visibility: PUBLIC
status: PUBLISHED
description: Everything you save in Pieces lives locally first. Here’s exactly where to find it—and how to share the right files when you need help.
metaTitle: Pieces On-Device Storage & Logs | Secure Data Guide
metaDescription: Learn where Pieces stores your database and logs on macOS, Windows, and Linux. Backup, restore, or delete data locally with SOC 2-certified security.
---

## Why it Matters

Pieces was designed with a **local-first architecture**—which is why all processing—code analysis, secret detection, and tag generation—runs completely offline by **default**:

* **What stays Local:** Snippets, tags, embeddings, LTM-2.7 memory, user settings, preferences, activity logs, diagnostic logs, and Pieces Copilot Chat history.

* **When it can move to the Cloud:** Only if you explicitly enable **Personal Cloud** or use a cloud-based model provider like OpenAI. In those cases, data is handled according to the provider’s privacy policy—not ours.

This architecture puts you in full control of your data, simplifies backup and restore, and minimizes your exposure to risk.

Cloud features are not required, are opt-in only, are isolated per user (`<your-subdomain>.pieces.cloud`).

We never use your data to train third-party models. You can delete your entire database, logs, and backups at any time by removing the `com.pieces.os` folder—more on that below.

<Callout type="tip">
  We’re **SOC 2 Type II** certified and never use your private data to train models.
</Callout>

## Where your Database Lives

Pieces stores all snippet metadata, embeddings, tags, and workflow context captured by LTM-2.7 in a single folder inside the `com.pieces` directory on your machine. 

| **Platform** | **Default path\***                             |
| ------------ | ---------------------------------------------- |
| *macOS*      | `/Users/<username>/Library/com.pieces.os/`     |
| *Windows*    | `C:/Users/<username>/Documents/com.pieces.os/` |
| *Linux*      | `/home/<username>/.local/share/com.pieces.os/` |

<Callout type="tip">
  Replace `<username>` with your OS account name.
</Callout>

Inside `com.pieces.os`, you’ll see `production`, which contains several folders that store broken down LTM-2.7 context and the rest of your data.

You are free to **copy, compress,** or **relocate** the entire `production` folder—for example, to sync via OneDrive or to migrate to another machine.

### Finding your Logs

When you open a GitHub issue or contact **Pieces Support**, attaching the most recent logs helps us diagnose problems in *minutes* instead of *hours*.

| **Platform** | **Log Directory**                                                     |
| ------------ | --------------------------------------------------------------------- |
| *macOS*      | `/Users/<username>/Library/com.pieces.os/production/support/logs/`    |
| *Windows*    | `C:/Users/<username>/Documents/com.pieces.os/production/support/logs` |
| *Linux*      | `/home/<username>/.local/share/com.pieces.os/logs/`                   |

Logs rotate daily and are timestamped (`log-05062025`).

Zip the latest two or three files and drag them into your <a target="_blank" href="https://github.com/pieces-app/support/issues">GitHub issue</a> or Discord DM with our engineers.

## Backup, Restore, or Reset

There are several options to backup, restore or reset your database from within the `com.pieces.os` folder.

| **Task**                                           | **Quick Steps**                                                                                                                                              |
| -------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| *Create a Manual Backup*                           | Quit all Pieces apps. Copy the entire `com.pieces.*` folder to your backup location, such as a USB drive, NAS, or cloud storage.                             |
| *Restore Database on a New Machine*                | Install Pieces OS. Replace the newly created `com.pieces.*` folder with your backup. Then, restart Pieces.                                                   |
| *Start Fresh or Troubleshoot a Corrupted Database* | Quit Pieces. Rename the `production` folder to something else, then relaunch. Pieces will create a brand-new, empty database (keep the backup just in case). |

## Need Help?<a target="_blank" href="/products/support">**​**</a>

You can open GitHub issues for PiecesOS, the Pieces Desktop App, or any other Pieces plugin or extension by <a target="_blank" href="https://github.com/pieces-app/support/issues">opening an issue in our GitHub repository.</a>

If you would prefer not to use GitHub, you can still <a target="_blank" href="https://getpieces.typeform.com/to/mCjBSIjF#page=docs-support">leave feedback or report a bug here.</a>
