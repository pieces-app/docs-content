---
title: Account & Cloud
path: /desktop/configuration/account-and-cloud
visibility: PUBLIC
status: PUBLISHED
description: The Account & Cloud settings allows you to manage third-party account connections, cloud synchronization, backups, your personal domain, and more.
metaTitle: Account and Cloud Configuration in the Pieces Desktop Application
metaDescription: The Account & Cloud settings allows you to manage third-party account connections, cloud synchronization, backups, your personal domain, and more.
---

## Accessing Settings

To open the **Account & Integration** and **Personal Cloud** settings, hover over your username in the top left, then hover over `Settings` and select either:

1. **Account & Integrations**: Manage external account connections and sign into or out of your Pieces account.

2. **Personal Cloud**: Connect to or disconnect from your Personal Cloud, manage backups, and edit the URL of your personal domain.

## Account Management

External account connections in Pieces are managed through third-party services such as Microsoft, Google, or GitHub.

### Viewing & Editing Linked Accounts

You can connect or disconnect third-party services from this modal.

* View connected accounts (GitHub, Google, Microsoft).

* Accounts are linked upon sign-in and cannot be manually edited.

* Profile information (name, email, avatar) is pulled from the linked service.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Account%20%26%20Cloud/account_integrations.png" alt="" align="center" fullwidth="true" />

## Personal Cloud

Pieces can run entirely offline, but connecting to Pieces Cloud enables real-time syncing and access across devices.

### Cloud Syncing

Cloud syncing is *optional.*

Once connected, syncing is automatic and happens in real time. Once connected, the only way to disable syncing is by disconnecting from Pieces Cloud.

<Callout type="tip">
  Any material saved in **Pieces Drive** or marked as a snippet is backed up. There are *no storage limits* on cloud-synced data.
</Callout>

### Disconnecting Personal Cloud

You can disconnect from your *Personal Cloud* at anytime by clicking the slashed `Cloud` icon, which opens up a *Disconnect Cloud* modal.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Pieces%20Copilot/Configure/disconnect_cloud.png" alt="" align="center" fullwidth="true" />

There are several features which require connectivity to your *Personal Cloud,* so be sure to read through these before disconnecting:

1. **Link Sharing:** The ability to generate and share links for saved materials from the **Pieces Drive.**

2. **Cloud ML:** Cloud-based enrichment of metadata for saved materials.

3. **Cloud Backup:** The automatic synchronization of your data to Pieces Cloud.

4. **Cloud Integrations:** Your Pieces Cloud which controls your personal subdomain and other integrations.

### Backup & Restore

Pieces allows *manual backups* of your data for long-term storage and recovery.

These data backups are *not automatic* and must be manually created. To create a backup:

<Steps>
  <Step title="Access Personal Cloud Settings">
    Click on your username in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Open Backup Manager">
    Click the **Backup & Restore** icon to open the backup menu.
  </Step>

  <Step title="Create Backup">
    Click `Create Backup` to save a snapshot and upload it to Pieces Cloud.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/desktop_app_assets/desktop_app_MAIN/new_media/Settings/Account%20%26%20Cloud/backup_restore.png" alt="" align="center" fullwidth="true" />

### Backup Contents

A Pieces backup contains the following data:

| **Data Type**           | **Summary**                                                       |
| ----------------------- | ----------------------------------------------------------------- |
| *Snippets*              | All saved code snippets and related metadata.                     |
| *Pieces Drive Files*    | Any files stored in Pieces Drive.                                 |
| *User Preferences*      | Theme, UI settings, and personalization options.                  |
| *Pieces Copilot Data*   | Recent chat history and AI context for Pieces Copilot.            |
| *Search & Tagging Data* | User-defined tags and previous searches for quick retrieval.      |
| *Account Connections*   | Linked GitHub, Google, or Microsoft accounts (without passwords). |

<Callout type="alert">
  Backups *do not include* Pieces Cloud data that is already synced or external files which are not explicitly stored in Pieces Drive.
</Callout>

### Restoring a Backup

Previous backups are listed in the **Backup Manager** with details including:

1. **Timestamp** of when the backup was created.

2. **File size** of the backup.

3. **Device name** that created the backup.

4. **PiecesOS version** at the time of backup.

Clicking the `Restore` icon will recover all saved materials, settings, and preferences and return Pieces Drive and the Pieces Desktop App to that previous state.

### Deleting a Backup

To delete a backup, click the `Trash` icon. Note that, when a backup is deleted, it *cannot be restored.* This is a permanent deletion.

## Personal Domain

When you’re connected to Pieces Cloud, you’re assigned a personal subdomain (e.g., [yourname.pieces.cloud](http://yourname.pieces.cloud)) for sharing snippets.

This subdomain isn’t publicly browsable like a profile page—instead, it’s prepended to any URLs you generate when sharing saved materials.

You can customize your subdomain at any time. To do so, open **Settings,** then **Personal Cloud**, and edit the input field under **Personal Domain**.