---
title: Get Started
path: /extensions-plugins/jetbrains/get-started
visibility: PUBLIC
status: PUBLISHED
description: Follow the steps below to install and use the Pieces for JetBrains Plugin.
metaTitle: Getting Started with Pieces for JetBrains | Pieces Docs
metaDescription: Get started with Pieces for JetBrains Plugins—install, configure, and enhance your workflow with AI-powered coding assistance.
---

<pieces-pro-cta />

## JetBrains Prerequisites

Before you begin, make sure you have:

* **PiecesOS:** The core engine that powers all Pieces extensions. <a target="_blank" href="/products/core-dependencies/pieces-os">Learn more about PiecesOS.</a>

* **Any JetBrains IDE:** The <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> works with any of the official JetBrains IDEs, so make sure you’ve got one installed.

You must have <a target="_blank" href="/products/core-dependencies/pieces-os">PiecesOS</a> to use the Pieces for JetBrains Plugin. We also recommend downloading the Pieces for Developers Desktop App.

### Sign in Required

Pieces requires all users to sign in before using any plugins or extensions. You'll be prompted to authenticate if you haven't already. For help, see our [sign-in guide](/products/meet-pieces/sign-into-pieces).

## Installing the Pieces for JetBrains Plugin

You can install the Pieces for JetBrains plugin through the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces--save-search-share--reuse-code-snippets">JetBrains Marketplace</a> or by searching for Pieces in the plugins search of your IDE.

<Image src="https://cdn.hashnode.com/res/hashnode/image/upload/v1731511626110/c73ee89d-099b-4dd4-b438-263777362657.png" alt="" align="center" fullwidth="true" />

Once you've installed the plugin, you can use Pieces without restarting your IDE.

### Setting up PiecesOS

<a target="_blank" href="/products/core-dependencies/pieces-os">PiecesOS</a> is required for the <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> to work.

If you haven’t installed it yet, click the buttons to download PiecesOS via the recommended method, or follow the alternative steps below.

<get-started-install />

<Callout type="alert">
  For enhanced security and better system integration, we recommend installing the `appinstaller` package over the InnoSetup (.exe) installer. The `appinstaller` package operates in a containerized environment, providing additional security benefits.
</Callout>

## Updating

The <a target="_blank" href="https://plugins.jetbrains.com/plugin/17328-pieces">Pieces for JetBrains Plugin</a> will automatically update when a new version is available.

When the plugin updates, a small success message will appear in the bottom right-hand corner of your JetBrains IDE.

<Callout type="tip">
  **Update notifications** cover updates for both the Pieces for JetBrains Plugin and PiecesOS.
</Callout>

You can also manually update the plugin by going to[ ](https://builds.pieces.app/stages/production/appinstaller/pieces_for_x.appinstaller?download=true\&product=DOCUMENTATION_WEBSITE)your Plugins window, locating the Pieces for JetBrains Plugin, and clicking the `Update` button.

## Pieces Cloud

<Callout type="info">
  Connecting to the Pieces Cloud is optional. However, it **provides additional features** like **data backups, shareable links, and more.** You can enjoy the main functionalities of Pieces without an account.
</Callout>

Disconnecting from the Pieces Cloud logs you out of your Pieces account.

To disconnect from the Pieces Cloud:

<Steps>
  <Step title="Open the Command Palette">
    Open the command palette in VS Code with `⌘+shift+p` (macOS) or `ctrl+shift+p` (Windows/Linux)
  </Step>

  <Step title="Disconnect from the Cloud">
    Enter `Disconnect from Pieces Cloud` and choose the option
  </Step>
</Steps>

<Callout type="info">
  If you’re not signed into Pieces Cloud - this option will not be available. You will see `Connect to Pieces Cloud`.
</Callout>

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/get_started/disconnect_pieces_cloud.gif" alt="" align="center" fullwidth="true" />

## Onboarding

The Pieces for JetBrains plugin features an interactive walkthrough that shows all the steps in one panel. This onboarding page teaches you how to save, view, and use saved materials, and how to get the most out of the Pieces for JetBrains plugin.

<Callout type="alert">
  If you don’t have PiecesOS installed, the Pieces for JetBrains plugin onboarding will require you to install it before completing the onboarding steps.
</Callout>

### Save Your First Material

Click `Save Your First Material`, and Pieces will automatically open the [Pieces Drive](/products/extensions-plugins/jetbrains/drive) to save a sample snippet, showing you how it all works.

You'll see that snippet right away in the **Saved Materials** list. This shows how Pieces captures items and keeps them organized for easy reuse.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/get_started/save_first_material" alt="" align="center" fullwidth="true" />

### View Your Saved Materials

Click `View Your Saved Materials`, and Pieces Drive will open to your **Saved Materials**, showing any snippets you saved earlier along with the new snippet.

### Check Out the Pieces Copilot

Click `Open Your Copilot` to open the Pieces Copilot side panel, as shown in the screenshots. In the Pieces Copilot, you'll find **suggested prompts**, options to set context from folders or files, and quick links to your saved materials.

Once you open the Copilot, the onboarding step is complete. You're ready to ask [questions about your code](/products/extensions-plugins/jetbrains/copilot/chat), [document it](/products/extensions-plugins/jetbrains/copilot/documenting-code), [debugging](/products/extensions-plugins/jetbrains/copilot/debugging-errors), or [refactor a selected material](/products/extensions-plugins/jetbrains/copilot/refactoring)—all within the JetBrains interface.

### Ask Copilot with Your Material

Click `Ask Copilot about Your Material`, and Pieces will add the new snippet to the Copilot chat with the sample prompt “What does this code do?”. Press `Enter` to send your snippet to the Copilot, and you'll receive an explanation or suggestions about the snippet.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/get_started/ask_copilot_about_material.gif" alt="" align="center" fullwidth="true" />

### Supercharge Your Workflow

Click `Pieces Documentation` to access our complete guide, which includes advanced tips, setup instructions, and best practices. Select `View All Steps` to revisit any onboarding step whenever you like.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/get_started/supercharge_workflow.png" alt="" align="center" fullwidth="true" />

<Callout type="info">
  If you need extra support, you can find [helpful resources here](/products/support).
</Callout>

## Uninstalling

To uninstall the Pieces for JetBrains Plugin, go to the `Settings` icon in the top left, `Plugins > Installed`, find the Pieces plugin, and click the uninstall button in the dropdown menu.

<Callout type="info">
  To access the uninstall option, click the dropdown menu and select the chevron to display the uninstall button.
</Callout>

You'll need to restart the JetBrains IDE for Pieces to be completely uninstalled.

<Image src="https://storage.googleapis.com/hashnode_product_documentation_assets/jetbrains_plugin_assets/jetbrains_plugin_assets/get_started/uninstall_button.png" alt="" align="center" fullwidth="true" />