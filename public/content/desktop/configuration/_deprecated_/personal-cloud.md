---
title: Personal Cloud
path: /desktop/configuration/personal-cloud
visibility: PUBLIC
status: PUBLISHED
description: Configure Personal Cloud settings for synchronization, backups, and personal domain management.
metaTitle: Personal Cloud Settings in Pieces Desktop
metaDescription: Configure Personal Cloud settings for synchronization, backups, and personal domain management.
---

***

## Personal Cloud Settings

Configure cloud synchronization, backups, and your personal domain. This keeps your materials and workflow history available wherever you work.

To access Personal Cloud settings, click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.

Pieces can run entirely offline, but connecting to Pieces Cloud enables real-time syncing and access across devices. This keeps your materials, settings, and workflow history available wherever you work.

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Personal Cloud settings showing disconnected status with connection options

## Connecting to Personal Cloud

Connect to your Personal Cloud to enable cloud synchronization, backups, and sharing features. When you connect, Pieces will automatically sync if you already have a cloud account, or create a new cloud for you.

### Connecting Your Cloud

<Steps>
  <Step title="Open Personal Cloud Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Click Cloud Icon">
    When your cloud is disconnected, click the `Cloud Icon` to the right of the status indicator to connect to your Personal Cloud.
  </Step>

  <Step title="Automatic Connection">
    Pieces will automatically sync your data if you already have a cloud account, or create a new cloud account for you. Once connected, your status will update to "Connected" and you'll have access to all cloud features.
  </Step>
</Steps>

<Callout type="tip">
  Any material saved in *Pieces Drive* or marked as a snippet is backed up. There are *no storage limits* on cloud-synced data.
</Callout>

## Cloud Status

View your cloud connection status and when it was last updated. The status indicator shows whether your Personal Cloud is connected or disconnected, along with a timestamp of the last update.

### Viewing Cloud Status

<Steps>
  <Step title="Open Personal Cloud Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Check Status">
    At the top of the Personal Cloud settings, you'll see your connection status:
    * **Connected**: Shows "Status: Connected" with a green dot, along with "Last updated [time]" 
    * **Disconnected**: Shows "Status: Disconnected" with a gray dot
  </Step>
</Steps>

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Personal Cloud settings showing connected status with personal domain and backup options

## Disconnecting Personal Cloud

Disconnect from your Personal Cloud at any time to disable cloud synchronization and features. You can reconnect later if needed.

### Disconnecting Your Cloud

<Steps>
  <Step title="Open Personal Cloud Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Click Disconnect Icon">
    When your cloud is connected, click the `Disconnect Cloud Icon` (cloud with diagonal line) to disconnect from your Personal Cloud.
  </Step>

  <Step title="Confirm Disconnection">
    Confirm the disconnection when prompted. Once disconnected, cloud features will be disabled and your status will show as "Disconnected".
  </Step>
</Steps>

Before disconnecting, keep in mind that several features require connectivity to your Personal Cloud:

* **Sharing (beta)**: The ability to generate and share links for saved materials from Pieces Drive
* **Cloud ML**: Cloud-based enrichment of metadata for saved materials
* **Cloud Backup**: The automatic synchronization of your data to Pieces Cloud
* **Cloud Integrations**: Your Pieces Cloud which controls your personal subdomain and other integrations

## Personal Domain

Customize your personal subdomain to create a unique URL for sharing your materials. Your personal domain is used when generating shareable links for your saved materials.

### Understanding Personal Domains

When you're connected to Pieces Cloud, you're assigned a personal subdomain (e.g., `yourname.pieces.cloud`) for sharing snippets. This subdomain isn't publicly browsable like a profile page—instead, it's prepended to any URLs you generate when sharing saved materials.

### Customizing Your Personal Domain

Create a custom subdomain by entering any text you want before `.pieces.cloud` to make `your_custom_url.pieces.cloud`.

<Steps>
  <Step title="Open Personal Cloud Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Locate Personal Domain Section">
    Scroll to the *Personal Domain* section, which shows your current domain status and the text input field.
  </Step>

  <Step title="Enter Custom Subdomain">
    In the text input field, enter the custom text you want to use before `.pieces.cloud`. For example, entering "nolanworksat" will create `nolanworksat.pieces.cloud`.
  </Step>

  <Step title="Save Changes">
    Your domain will update automatically. The section will show "Your domain [your_custom_url].pieces.cloud is running" when active.
  </Step>
</Steps>

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Personal Domain section showing custom subdomain input and active domain status

## Backup & Restore Data

Create manual backups of your data for long-term storage and recovery. These backups are stored in your personal Pieces cloud and can be restored or deleted at any time.

### Opening Backup & Restore Data

Access the backup management interface to create backups, view existing backups, restore previous versions, or delete old backups.

<Steps>
  <Step title="Open Personal Cloud Settings">
    Click your `User Profile` in the top left, then hover over `Settings` and select `Personal Cloud`.
  </Step>

  <Step title="Click Restore Icon">
    In the *Backup & Restore Data* section, click the `Restore Icon` (Circular Arrow Icon) to open the Backup & Restore Data modal.
  </Step>
</Steps>

<Image src="https://www.jacksonsquareshopping.co.uk/wp-content/uploads/2016/12/placeholder-1920x1080-copy.png" alt="" align="center" fullwidth="true" />

> Backup & Restore Data modal showing backup list, create backup option, and Check for Backups button

### Checking for Backups

Manually check for new backups that may have been created from other devices or sessions.

<Steps>
  <Step title="Open Backup & Restore Data Modal">
    Click your `User Profile` in the top left, hover over `Settings`, select `Personal Cloud`, then click the `Restore Icon` in the *Backup & Restore Data* section.
  </Step>

  <Step title="Click Check for Backups">
    In the top right of the modal, click the `Check for Backups` button (Refresh Icon) to manually check for any new backups.
  </Step>
</Steps>

### Creating a Backup

Create a manual backup snapshot of your data. Backups are stored in your personal Pieces cloud and include all your saved materials, settings, and preferences.

<Steps>
  <Step title="Open Backup & Restore Data Modal">
    Click your `User Profile` in the top left, hover over `Settings`, select `Personal Cloud`, then click the `Restore Icon` in the *Backup & Restore Data* section.
  </Step>

  <Step title="Locate Create Backup Section">
    In the modal, find the *Create Backup* section, which shows "Backups will be stored in your personal Pieces cloud".
  </Step>

  <Step title="Click Create Backup">
    Click the `Cloud Icon with Upward Arrow` to create a new backup. The backup will be created and uploaded to your personal Pieces cloud.
  </Step>
</Steps>

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

### Viewing Your Backups

See all of your available backups with details about when they were created, their size, the device they were created on, and the PiecesOS version at the time of backup.

<Steps>
  <Step title="Open Backup & Restore Data Modal">
    Click your `User Profile` in the top left, hover over `Settings`, select `Personal Cloud`, then click the `Restore Icon` in the *Backup & Restore Data* section.
  </Step>

  <Step title="Review Backup List">
    Scroll down to the *Backups* section, which shows the total number of backups and lists each backup with:
    * **Date and time**: When the backup was created (e.g., "Mon, Dec 8, 2025 9:41 AM")
    * **Size**: The backup file size (e.g., "342.85 MB")
    * **Device**: The device name where the backup was created (e.g., "Judsons MacBook Air")
    * **OS Version**: The PiecesOS version at the time of backup (e.g., "PiecesOS v12.3.3")
  </Step>
</Steps>

### Restoring a Backup

Restore a previous backup to recover all saved materials, settings, and preferences. This will return Pieces Drive and the Pieces Desktop App to the state captured in that backup.

<Steps>
  <Step title="Open Backup & Restore Data Modal">
    Click your `User Profile` in the top left, hover over `Settings`, select `Personal Cloud`, then click the `Restore Icon` in the *Backup & Restore Data* section.
  </Step>

  <Step title="Locate Backup">
    In the *Backups* section, find the backup you want to restore from the list.
  </Step>

  <Step title="Click Restore Icon">
    Click the `Restore Icon` (Refresh/Circular Arrow Icon) on the right side of the backup entry to restore that backup.
  </Step>

  <Step title="Confirm Restoration">
    Confirm the restoration when prompted. All saved materials, settings, and preferences will be restored to the state captured in that backup.
  </Step>
</Steps>

### Deleting a Backup

Remove old backups that you no longer need. Deleted backups cannot be restored—this is a permanent deletion.

<Steps>
  <Step title="Open Backup & Restore Data Modal">
    Click your `User Profile` in the top left, hover over `Settings`, select `Personal Cloud`, then click the `Restore Icon` in the *Backup & Restore Data* section.
  </Step>

  <Step title="Locate Backup">
    In the *Backups* section, find the backup you want to delete from the list.
  </Step>

  <Step title="Click Delete Icon">
    Click the `Trash Icon` on the right side of the backup entry to delete that backup.
  </Step>

  <Step title="Confirm Deletion">
    Confirm the deletion when prompted. The backup will be permanently removed and cannot be restored.
  </Step>
</Steps>

## Cloud Syncing

Cloud syncing is optional—you can use Pieces entirely offline if you prefer. Once connected, syncing happens automatically in real time, keeping your data synchronized across all your devices. The only way to disable syncing is by disconnecting from Pieces Cloud.

When connected, your data is automatically synchronized in real time across all devices where you're signed in. This includes snippets, Pieces Drive files, settings, and workflow history.

***

## Next Steps

Now that you understand how to manage your Personal Cloud, learn about [Account](/products/desktop/configuration/account) settings to manage your authentication and linked accounts, or explore [Connected Applications](/products/desktop/configuration/connected-applications) to integrate Pieces with other services.
