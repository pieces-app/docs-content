---
title: Configuration
path: /extensions-plugins/jetbrains/configuration
visibility: PUBLIC
status: PUBLISHED
description: Read the guide below to configure the Pieces for JetBrains Plugin to work efficiently in your workflow and adapt to your preferences.
metaTitle: Configuring Pieces for JetBrains | Pieces Docs
metaDescription: Configure the Pieces for JetBrains Plugin to match your workflow and optimize how you manage, search, and interact with your saved snippets.
---

## Supported LLMs

We constantly update and configure our plugins and extensions, like the Pieces for JetBrains Plugin, to work with the latest LLMs.

The Pieces for JetBrains Plugin currently supports [54 different cloud and local models.](/products/large-language-models)

[Read documentation on how to switch the LLM](/products/extensions-plugins/jetbrains/copilot/llm-settings) utilized by the Pieces for JetBrains Plugin from within your IDE.

## Opening Pieces Settings

To access the **Pieces Settings** in the Pieces for JetBrains Plugin, click the `Pieces Settings` icon in your sidebar.

This action will open the Pieces Settings in a new sidebar.

## Overriding Commands in JetBrains

If you want to change the shortcuts for any Pieces functionality within your JetBrains IDE, like [saving a snippet](/products/extensions-plugins/jetbrains/drive/save-snippets#via-right-click-menu--hotkeys) or [generating a shareable link](/products/extensions-plugins/jetbrains/drive/sharing#how-to-share-a-saved-snippet), you can:

<Steps>
  <Step title="Open Settings">
    Navigate to **Settings** `⌘+,` (macOS) or `ctrl+,` (Windows/Linux).
  </Step>

  <Step title="Search for Keymap">
    Enter **Keymap** into the search bar.
  </Step>

  <Step title="Go to Plugins">
    Click on the Plugins section.
  </Step>

  <Step title="Locate Pieces Folder">
    Find the **Pieces** folder towards the bottom of the list (in alphabetical order).
  </Step>

  <Step title="Open Pieces Function">
    **Double-click** or **press** `return` or `enter` on a Pieces function.
  </Step>

  <Step title="Assign Keyboard Shortcut">
    Select `Add Keyboard Shortcut` and enter your preferred key mapping.

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/configuration/change_keybinds.gif" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

## Checking Your JetBrains IDE Version

You can easily check the version of your JetBrains IDE by opening up the **Settings** page using `⌘+,` (macOS) or `ctrl+,` (Windows/Linux) and searching for **Updates** under **System Settings.**

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/cdn_migrate_repair_2/jetbrains_ide_version_check.png" alt="" align="center" fullwidth="true" />

## Settings Overview

Several other configurable settings related to the functionality of the Pieces for JetBrains Plugin directly affect the usability of some of the plugin’s features. You can also enable or disable several preferences.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/configuration/new_settings_menu.png" alt="" align="center" fullwidth="true" />

### Account & Cloud Integrations (Beta)

Opened through the Pieces **Settings** sidebar or via the **Extensions** menu. This section displays your account details and beta-program status.

* **Account Name**: The display field showing your user name.

* **Account Email**: A display field showing your email address.

* **Early Access Program**: an indicator showing whether you’re enrolled in the beta program.

### Personal Cloud (Beta)

Manage your connection to the Pieces personal cloud.

* **Status**: An indicator + timestamp showing whether your personal cloud is **connected or disconnected**, and when it was last updated.

* **Personal Domain**: A display field with your custom subdomain (e.g., `<your-domain>.`[`pieces.cloud`](http://pieces.cloud)).

* **Backup & Restore Data**: A button to back up or restore your cloud data.

### Saved Material Auto-Enrichment

Configure how much context is automatically added when saving snippets.

* **Auto-Generated Context**: The dropdown allows you to select the level of auto-generated context (**None**, **Low**, **Medium**, **High**).

### ML Processing

Control which AI models and memory engine the extension uses.

* **Processing Mode**: A dropdown to choose **Local**, **Cloud**, or **Blended** processing; includes a brief description of resource usage.

* **Long-Term Memory Engine**: Toggle to enable/disable; auto-generates Workstream Activities and provides temporal context.

* **Long-Term Memory Source Control**: A button to manage which memory sources the engine interacts with.

* **Clear Long-Term Memory Engine Data…**: A button to purge persisted memory for a specified date range.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/configuration/ml_processesing_blendmode.png" alt="" align="center" fullwidth="true" />

### Model Context Protocol (MCP)

Configure your local MCP server connection.

* **Server URLs**: A text field listing the Pieces MCP endpoint URLs (e.g.\
  `http://localhost:39300/model_context_protocol/2024-11-05/sse`).

* **View Documentation**: A link to the MCP usage documentation.

<Callout type="alert">
  Currently, the JetBrains IDE Suite does not support the SEE protocol Pieces uses.
</Callout>

### CodeLenses

Manage the integration with VS Code’s CodeLens UI.

* **Enable Pieces Code-Lens**: A checkbox to enable or disable code-lens features.

* **Use Same Conversation For Code-Lens**: A checkbox to share the Copilot conversation across all code-lens actions.

### Code Block Actions

Determine how code execution commands are handled.

* **Use Integrated Terminal**: A checkbox to run “Run In Terminal” commands in the IDE’s integrated terminal instead of an external shell.

### Saved Materials

Settings related to snippet-saving behavior.

* **Close Snippet Editor on Save**: A checkbox to automatically close the snippet editor tab when saving.

* **Enable Automatic Link Copy**: A checkbox to copy the generated snippet link to your clipboard automatically.

### PiecesOS Configs

Configure how PiecesOS launches alongside your IDE.

* **Launch on Startup**: The checkbox automatically starts PiecesOS when VS Code launches.

* **Auto Launch on Interaction**: A checkbox to start PiecesOS the first time you interact with the extension.

### Autocomplete

Enable snippet completion suggestions.

* **Enable AutoComplete**: A checkbox to suggest saved snippets as you type.

### Git Integration

Configure metadata extraction from your Git history.

* **Pieces › Save › Git: Related Links**: A checkbox to attach commit links when saving a snippet.

* **Pieces › Save › Git: Related People**: A checkbox to attach commit authors when saving a snippet.

* **Pieces › Save › Git: Description**: A checkbox to use commit messages as snippet descriptions.

* **Pieces › Save › Git: Tags**: A checkbox to attach Git tags when saving a snippet.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/configuration/git_integration.png" alt="" align="center" fullwidth="true" />

### Notifications

Control update notifications for the extension.

* **Show Update Extension Notification**: A checkbox to prompt on startup if the extension is outdated.

### Onboarding

Manage the first-run tutorial state.

* **Reset Onboarding**: A button to clear the onboarding state on next launch.

* **Launch Onboarding**: A button to reopen the onboarding tutorial immediately.

### Telemetry & Analytics

Manage data-sharing preferences.

* **Telemetry & Diagnostics**: A checkbox to share anonymous telemetry and crash data.

* **Share Error Analytics**: A checkbox to share error reports to help improve Pieces.

* **Share Usage Analytics**: A checkbox to share feature-usage metrics to help improve Pieces.

### Support

Quick links to help and feedback.

* **Documentation**: This link will take you to online documentation.

* **Submit Feedback/Issues**: This link will take you to the GitHub issues page or support form.

### PiecesOS Information

Displays version and connection details for PiecesOS.

* **PiecesOS Version**: The display field shows the current version number.

* **Check for PiecesOS Updates**: A button to manually check for updates.

* **PiecesOS Port**: The display field shows the port on which PiecesOS is listening.

### Settings Applet

Shows the applet version for the extension settings.

* **Version**: A display field showing the current Settings Applet version number.