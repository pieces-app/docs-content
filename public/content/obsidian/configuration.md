---
title: Configuration
path: /obsidian/configuration
visibility: PUBLIC
status: PUBLISHED
description: Read the guide below to configure the Pieces for Obsidian Plugin to work efficiently in your workflow and adapt to your preferences.
metaTitle: How to Configure Pieces for Obsidian | Pieces Docs
metaDescription: Learn how to configure Pieces for Obsidian to tailor AI-powered features, snippet management, and workflow integrations to your needs.
---

## Supported LLMs

We constantly update and configure our plugins and extensions, like the Pieces for Obsidian Plugin, to work with the latest LLMs.

The Pieces for Obsidian Plugin supports 13 different cloud models and [41 local models](/products/large-language-models).

[Read the documentation on switching your Pieces Copilot Runtime (LLM)](/products/obsidian/copilot/llm-settings#how-to-configure-your-llm-runtime) utilized by the Pieces for Obsidian Plugin within your editor.

## Opening Pieces Settings

To open the Pieces Settings in the Pieces for Obsidian Plugin, select the `Pieces` icon in the left-hand sidebar and the `setting` icon in the new Pieces popup on the right side.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/configuration/open_settings.gif" alt="" align="center" fullwidth="true" />

## Overriding Commands in Obsidian

If you’d like to adjust the keyboard shortcuts for the Pieces for Obsidian Plugin, such as saving a snippet or previewing markdown, follow these steps:

<Steps>
  <Step title="Open Settings">
    Access the settings menu in Obsidian by clicking the gear icon in the lower-left corner.
  </Step>

  <Step title="Go to Hotkeys">
    Navigate to the "Hotkeys" tab in the settings menu to view or customize command shortcuts.
  </Step>

  <Step title="Find the Command">
    Use the search bar to locate the specific command you want to override, such as commands for the "Pieces" plugin.
  </Step>

  <Step title="Customize the Shortcut">
    Click on the current shortcut next to the command and input your preferred key combination to override it.
  </Step>

  <Step title="Save Changes">
    Ensure the new shortcut is displayed and test it to confirm the override is successful.
  </Step>
</Steps>

## Settings Overview

Below is a breakdown of each adjustable setting (preferences, behaviors, views, etc.) in the Pieces for Obsidian Plugin, updated based on available features.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/configuration/general_overview_obsid.png" alt="" align="center" fullwidth="false" />

### Account & Cloud Integrations

* **Account Name:** Displays the name associated with your Pieces for Obsidian account.

* **Account Email:** Displays the email address linked to your Pieces account.

* **Early Access Program:** Indicates whether you are enrolled in the beta program.

### Personal Cloud

* **Status:** Shows whether your personal cloud is connected or disconnected and when it was last updated.

* **Personal Domain:** Displays your custom subdomain and indicates that it is running.

* **Backup & Restore Data:** Opens a dialog to back up or restore your personal cloud data.

### Saved Material Auto-Enrichment

* **Auto-Generated Context:** This option lets you select how much context is auto-generated for saved materials (None, Low, Medium, High).

### ML Processing

* **Processing Mode:** Selects Local, Cloud, or Blended machine-learning resources.

* **Long-Term Memory Engine:** Toggles the on-device memory engine on or off and displays its current version.

* **Long-Term Memory Source Control:** Opens controls to manage which memory sources feed your long-term memory.

* **Clear Long-Term Memory Engine Data…:** Purges persisted memory data for a specified time range.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/obsidian_plugin_assets/configuration/ml_mode.png" alt="" align="center" fullwidth="false" />

### Model Context Protocol (MCP)

* **Server URLs:** Allows you to specify the URLs of your MCP endpoints.

* **Version:** Displays the MCP protocol version in use.

* **View Documentation:** Opens the MCP usage documentation.

### Saved Materials

* **Auto-Open Pieces Drive view on snippet save:** Automatically opens the Pieces Drive view when you save a snippet.

* **Use note page title for saved snippet:** When saving, your current note’s title is used as the snippet title.

### Onboarding

* **Launch Onboarding:** Reopens the onboarding tutorial at any time.

### Telemetry

* **Telemetry & Diagnostics:** Shares anonymized usage and crash data to help improve Pieces.

### Support

* **Documentation:** Opens the online Pieces documentation.

* **Submit Feedback/Issues:** The feedback or issue tracker is open for reporting bugs and requesting features.

### PiecesOS Information

* **PiecesOS Version:** Displays the installed version of the PiecesOS service.

* **Check for PiecesOS Updates:** Checks for and installs updates to PiecesOS.

* **PiecesOS Port:** Displays the network port on which PiecesOS is listening.

### Settings Applet

* **Version:** Displays the version number of the settings applet.

***

For additional support resources, check out our [troubleshooting guide.](/products/obsidian/troubleshooting)