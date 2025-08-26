---
title: Configuration
path: /extensions-plugins/visual-studio/configuration
visibility: PUBLIC
status: PUBLISHED
description: Refer to the guide below to effectively configure the Pieces for Visual Studio Extension to suit your workflow and personal preferences.
metaTitle: How to Configure the Pieces for Visual Studio Extension
metaDescription: Customize the Pieces for Visual Studio Plugin settings to enhance your development experience and workflow efficiency.
---

# Configuring PiecesOS

Read the documentation below on configuring PiecesOS with the Pieces for Visual Studio Extension to customize it to your exact needs.

## Supported LLMs

We continuously update and optimize our plugins and extensions to [ensure compatibility with the latest LLMs](/products/large-language-models).

[Read the documentation to learn how to switch your Pieces Copilot Runtime (LLM)](/products/extensions-plugins/visual-studio/copilot/llm-settings) used by the Pieces for Visual Studio Extension directly within your IDE.

## Opening Pieces Settings

To open the Pieces Settings in the **Pieces for Visual Studio Extension**, follow these steps:

<Steps>
  <Step title="Open the Views Dropdown">
    In the top left of the window, hover over `Views`, then hover over `Other Windows`, and lastly hover over `Pieces`.
  </Step>

  <Step title="Open and Adjust Settings">
    Select `Pieces Settings` view option. A new window will open in your solutions explorer for your Pieces settings.
  </Step>
</Steps>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/configuration/pieces_new_settings.png" alt="" align="center" fullwidth="true" />

## Overriding Commands in Visual Studio

To modify the keyboard shortcuts for Pieces functionality in Visual Studio, such as <a target="_blank" href="/products/extensions-plugins/visual-studio/drive/save-snippets">saving a snippet</a> or [launching the Copilot](/products/extensions-plugins/visual-studio/copilot/chat#accessing-copilot-chat-in-vs-code), follow these steps:

<Steps>
  <Step title="Open the Options Menu">
    Navigate to `Tools > Options` from the top toolbar in Visual Studio
  </Step>

  <Step title="Access Keyboard Settings">
    In the **Options** window, expand the `Environment` section and select `Keyboard`
  </Step>

  <Step title="Search for a Pieces Command">
    Use the search bar to find the Pieces command you want to modify, such as `Pieces.SaveToPieces`
  </Step>

  <Step title="Assign a New Shortcut">
    Select the command from the list and enter your preferred shortcut in the `Press shortcut keys` field
  </Step>

  <Step title="Save Your Shortcut">
    Ensure your new shortcut doesn’t conflict with existing Visual Studio commands, then click `Assign` to save your changes

    <Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/commands/pieces_keybinds_visual_studio.png" alt="" align="center" fullwidth="true" />
  </Step>
</Steps>

This process enables you to customize keyboard shortcuts to fit your workflow seamlessly.

## Settings Overview

You can configure several settings related to the Pieces for Visual Studio Extension, which directly affect the usability of some features. You can also enable or disable various preferences.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/configuration/general_view.png" alt="" align="center" fullwidth="false" />

### Account & Cloud Integrations

* **Account Name:** Displays your chosen display name in the Pieces extension for Visual Studio.

* **Account Email:** Displays the email address linked to your Pieces account.

* **Early Access Program:** Indicates whether you are enrolled in the beta program.

### Personal Cloud

* **Status:** Shows whether your cloud is connected or disconnected and when it was last updated.

* **Personal Domain:** Displays your custom subdomain (for example, `<your-domain>.`[`pieces.cloud`](http://pieces.cloud)).

* **Backup & Restore Data:** Provides a button to back up or restore your cloud data.

### Saved Material Auto-Enrichment

* **Auto-Generated Context:** A dropdown menu allows users to select the level of context auto-enrichment (None, Low, Medium, High).

### ML Processing

* **Processing Mode:** You can choose between Local, Cloud, or Blended processing.

* **Long-Term Memory Engine:** Toggles the memory engine on or off and shows its current version.

* **Long-Term Memory Source Control:** Provides a button to manage which data sources feed into long-term memory.

* **Clear Long-Term Memory Engine Data…:** Provides a button to purge persisted memory for a specified date range.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/visual_studio_extension_assets/configuration/ml_blended.png" alt="" align="center" fullwidth="false" />

### Model Context Protocol (MCP)

* **Server URLs:** Provides a text field where you can list all of your MCP endpoint URLs.

* **View Documentation:** Links to the official MCP usage documentation.

### CodeLenses

* **Enable Pieces Code-Lens:** Toggles the code-lens features on or off in the editor.

* **Use Same Conversation For Code-Lens:** Shares a single Copilot conversation across all code-lens actions.

### Code Block Actions

* **Use Integrated Terminal:** Ensures that “Run In Terminal” uses Visual Studio’s integrated terminal instead of opening an external one.

### Saved Materials

* **Close Snippet Editor on Save:** Automatically closes the snippet editor when you save a snippet.

* **Enable Automatic Link Copy:** Automatically copies the snippet’s shareable link to your clipboard upon saving.

### PiecesOS Configs

* **Launch on Startup:** Automatically starts the PiecesOS background service when Visual Studio launches.

* **Auto Launch on Interaction:** Automatically starts PiecesOS the first time you interact with the extension.

### Autocomplete

* **Enable AutoComplete:** Suggests your saved snippets inline as you type code.

### Git Integration

* **Pieces › Save › Git: Related Links:** Attaches related commit links from your Git history when you save a snippet.

* **Pieces › Save › Git: Related People:** Attaches commit author information from your Git history when saving a snippet.

* **Pieces › Save › Git: Description:** Uses commit messages from your Git history as the default description for the snippet.

### Notifications

* **Show Update Extension Notification:** Prompts you at startup if a newer version of the extension is available.

### Onboarding

* **Reset Onboarding:** Resets the onboarding tutorial to run on the next launch.

* **Launch Onboarding:** Reopens the onboarding tutorial at any time.

### Telemetry & Analytics

* **Telemetry & Diagnostics:** Shares anonymous usage and crash data to help improve the extension.

* **Share Error Analytics:** Shares detailed error reports to help diagnose and fix issues.

* **Share Usage Analytics:** Shares anonymized feature-usage metrics to guide future development.

### Support

* **Documentation:** Provides a link to the online Pieces documentation.

* **Submit Feedback/Issues:** Provides a link to the feedback or issue tracker for reporting bugs and requesting features.

## PiecesOS Information

* **PiecesOS Version:** Displays the current version number of the PiecesOS service.

* **Check for PiecesOS Updates:** Provides a button to check for and install PiecesOS updates manually.

* **PiecesOS Port:** Displays the network port on which PiecesOS is listening.

## Settings Applet

* **Version:** Displays the current version number of the Settings Applet.

***

For additional support resources, check out our [troubleshooting guide.](/products/extensions-plugins/visual-studio/troubleshooting)

***